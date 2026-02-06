---
title: スクラムのためのソフトウェアエンジニアリングプラクティス（SGEPの拡張）
description: 効果的なソフトウェアエンジニアリングはスクラムが速いフィードバック、安全な変更、継続的にリリース可能なソフトウェアを提供することを可能にします。CI、CD、自動化、TDDなどのプラクティスを使って小さなテスト可能なステップで作業することで、チームはトレードオフなしに高い品質、スピード、適応性を達成します。
keywords:
  - スクラム
  - モダンスクラム
  - プロダクトマネジメント
  - モダンソフトウェアエンジニアリング
  - 継続的デリバリー
  - 開発プラクティス
author:
  - Dave Farley
translators:
  - Claude AI
  - Takeshi Kawaguti
date: 2026-01-18T09:00:00Z
type: guide
lang: ja
mainfont: "Times New Roman"
sansfont: "Arial"
monofont: "Courier New"
aliases:
  - /ja/software-engineering-practices/2026.1/
sitemap:
  priority: 0.7
---

<!-- **_Collected Resources for Scrum Guide Expansion Pack_**
_This document is a collection of independent works. Each section retains its original license or copyright status, as indicated. Please refer to each section for specific usage rights and requirements._ -->

**_Scrum Guide Expansion Packのための収集リソース_**

_この文書は独立した作品のコレクションです。各セクションは、示されているように、元のライセンスまたは著作権ステータスを保持しています。特定の使用権と要件については、各セクションを参照してください。_

<!-- **License/Copyright:** [CC BY-NC-ND 4.0](https://creativecommons.org/licenses/by-nc-nd/4.0/)
**Note:** This section is included in its original, unaltered form with permission under the terms of the [CC BY-NC-ND 4.0](https://creativecommons.org/licenses/by-nc-nd/4.0/) license. No changes have been made. -->

**ライセンス/著作権:** [CC BY-NC-ND 4.0](https://creativecommons.org/licenses/by-nc-nd/4.0/)

**注記:** このセクションは [CC BY-NC-ND 4.0](https://creativecommons.org/licenses/by-nc-nd/4.0/) ライセンスの条件に基づき、許可を得て原文のまま収録されています。変更は加えられていません。

---

<!-- Scrum is a framework for developing and sustaining complex products. It provides the structure within which Scrum Teams can deliver value iteratively and incrementally. Scrum does not specify how Scrum Teams should build products or which techniques they must use. However, Scrum requires Scrum Teams to execute this iterative, incremental work effectively. -->

スクラムは複雑なプロダクトを開発し維持するためのフレームワークです。スクラムチームが反復的かつ漸進的に価値を提供できる構造を提供します。スクラムはスクラムチームがどのようにプロダクトを構築すべきか、またはどの技術を使用すべきかを規定していません。しかし、スクラムはスクラムチームがこの反復的で漸進的な作業を効果的に実行することを要求します。

<!-- If the way work is organized does not support step-by-step learning, experimentation, and adaptation, many of Scrum's advantages disappear. That is why Scrum Teams and organizations must deliberately organize their work to encourage exploration, feedback, and continuous adjustment to succeed with Scrum. The quality and sustainability of outcomes depend on the engineering practices that Scrum Teams apply. -->

作業の組織化の方法がステップバイステップの学習、実験、適応をサポートしない場合、スクラムの多くの利点は消えてしまいます。そのため、スクラムチームと組織は、スクラムで成功するために、探索、フィードバック、継続的な調整を促進するように意図的に作業を組織化する必要があります。アウトカムの品質と持続可能性は、スクラムチームが適用するエンジニアリングプラクティスに依存します。

<!-- This document outlines essential engineering practices that enhance Scrum's effectiveness in software engineering for digital products (SGEP/ProductThinking). -->

この文書は、デジタルプロダクトのためのソフトウェアエンジニアリングにおけるスクラムの有効性を高める、不可欠なエンジニアリングプラクティスの概要を説明します（SGEP/ProductThinking）。

<!-- ## Purpose -->

## 目的 {#purpose}

<!-- The purpose of engineering practices within Scrum is to ensure that each Increment is in a usable state that enables learning and insight. What "high quality" means can change depending on the stage of development and the level of uncertainty in the product's environment. Engineering practices should therefore support releasing when it makes sense, learning quickly from real use, and helping the people doing the work sustain the ability to deliver reliable outcomes again and again over time. -->

スクラム内のエンジニアリングプラクティスの目的は、各インクリメントが学習と洞察を可能にする使用可能な状態にあることを保証することです。「高品質」が意味するものは、開発の段階やプロダクトの環境における不確実性のレベルによって変わる可能性があります。したがって、エンジニアリングプラクティスは、意味があるときにリリースすること、実際の使用から素早く学習すること、そして作業を行う人々が時間をかけて信頼性の高いアウトカムを何度も提供する能力を維持することをサポートすべきです。

<!-- Without a disciplined engineering approach, Scrum devolves into short cycles of poorly integrated work, which accumulate technical debt and reduce agility. -->

規律あるエンジニアリングアプローチがなければ、スクラムは統合が不十分な作業の短いサイクルに堕落し、技術的負債を蓄積してアジリティを低下させます。

<!-- ## The Case for "Engineering" -->

## 「エンジニアリング」の根拠 {#the-case-for-engineering}

<!-- In simple terms, supported by user access and their feedback, modern engineering is the practical side of empirical process control. It is about making things work in the real world. In many fields, "engineering" basically means "the stuff that works reliably." -->

簡単に言えば、ユーザーアクセスとそのフィードバックによってサポートされるモダンエンジニアリングは、経験的プロセス制御の実践的な側面です。それは現実世界で物事を機能させることについてです。多くの分野で、「エンジニアリング」は基本的に「信頼性のある動作をするもの」を意味します。

<!-- The purpose of engineering is not to find the one perfect solution. Instead, it helps rule out bad ideas and narrow the options to better ones. These options can then be compared to determine the best fit. -->

エンジニアリングの目的は、唯一の完璧な解決策を見つけることではありません。代わりに、悪いアイデアを排除し、選択肢をより良いものに絞り込むのに役立ちます。これらの選択肢は、最適なものを決定するために比較できます。

<!-- Engineering uses principles and practices that help people avoid common mistakes and weak solutions. Examples of this way of thinking include building in safety margins and designing systems that fail safely rather than causing damage. -->

エンジニアリングは、人々が一般的な間違いや弱い解決策を避けるのに役立つ原則とプラクティスを使用します。この考え方の例には、安全マージンを組み込むことや、損害を引き起こすのではなく安全に失敗するシステムを設計することが含まれます。

<!-- Engineering cannot guarantee success. However, it produces far better results than not using engineering at all. When this mindset is applied continuously, it helps Scrum Teams learn, improve, and gradually move toward better outcomes, which is exactly what makes inspect & adapt possible. -->

エンジニアリングは成功を保証できません。しかし、エンジニアリングを全く使用しないよりもはるかに良い結果を生み出します。このマインドセットが継続的に適用されると、スクラムチームが学習し、改善し、より良いアウトカムに向けて徐々に進むのを助けます。これはまさに検査と適応を可能にするものです。

<!-- So what are the software equivalent of "engineering" principles that can guide people towards those better outcomes? -->

では、人々をより良いアウトカムに導くことができる「エンジニアリング」原則のソフトウェア相当物は何でしょうか？

<!-- ## Principles -->

## 原則 {#principles}

<!-- Perhaps the most foundational principle in empirical process control, science, and engineering is the idea that one begins by assuming that one's guesses are probably wrong. -->

経験的プロセス制御、科学、エンジニアリングにおいておそらく最も基礎的な原則は、自分の推測はおそらく間違っているという仮定から始めるというアイデアです。

<!-- **Science is a satisfactory philosophy of ignorance**: _Because we have the doubt, we then propose looking in new directions for new ideas._
– Richard Feynman -->

**科学は無知についての満足のいく哲学である**: _疑いがあるからこそ、私たちは新しいアイデアを求めて新しい方向を見ることを提案する。_
– Richard Feynman

<!-- This is also fundamentally the philosophy behind agile development. One is permitted the freedom to make mistakes and organize the work so mistakes are detected as soon as possible. This idea encourages people to make progress in small, safe, verifiable steps, so they can check for mistakes after each step and correct any problems, whatever their nature. This idea is at the core of any sound engineering approach to software development and shapes how people think about and approach the work as a whole. -->

これは基本的にアジャイル開発の背後にある哲学でもあります。間違いを犯す自由が許され、間違いができるだけ早く検出されるように作業を組織化します。このアイデアは、人々が小さく、安全で、検証可能なステップで進歩することを奨励し、各ステップの後に間違いをチェックし、その性質が何であれ問題を修正できるようにします。このアイデアは、ソフトウェア開発への健全なエンジニアリングアプローチの中核にあり、人々が作業全体についてどのように考え、アプローチするかを形作ります。

<!-- It is important, however, to avoid becoming overly focused on the process alone. The ultimate goal of software development is to create value or utility for users. To succeed as an engineering discipline, the organization of work must reliably guide people toward outcomes that are more likely to deliver that value or utility. -->

しかし、プロセスだけに過度に集中することを避けることが重要です。ソフトウェア開発の究極の目標は、ユーザーのために価値や実用性を創造することです。エンジニアリング規律として成功するためには、作業の組織化が、その価値や実用性を提供する可能性が高いアウトカムに向けて人々を確実に導く必要があります。

<!-- So while customer value is the real goal, engineering practices in the context of Scrum share these common principles that will enable people to achieve the real goals of solving customer problems and discovering new opportunities: -->

したがって、顧客価値が真の目標である一方で、スクラムの文脈におけるエンジニアリングプラクティスは、顧客の問題を解決し新しい機会を発見するという真の目標を達成することを可能にする、これらの共通の原則を共有しています：

<!-- 1. **Enable Adaptiveness**: _enable rapid, safe change without compromising quality._
2. **Accelerate Feedback**: _reduce the time to discover errors or validate value._
3. **Increase Transparency**: _provide a clear picture of product quality and operational state._
4. **Support Sustainability**: _maintain a consistent (but sustainable) pace without compromising product quality._ -->

1. **適応性を可能にする**: _品質を損なうことなく、迅速で安全な変更を可能にする。_
2. **フィードバックを加速する**: _エラーを発見したり価値を検証したりする時間を短縮する。_
3. **透明性を高める**: _プロダクトの品質と運用状態の明確な画像を提供する。_
4. **持続可能性をサポートする**: _プロダクトの品質を損なうことなく、一貫した（しかし持続可能な）ペースを維持する。_

<!-- ### Enabling Adaptiveness through Technical Practices -->

### 技術的プラクティスを通じた適応性の実現 {#enabling-adaptiveness-through-technical-practices}

<!-- These principles are deeply interlinked, and at their heart lie the fundamentals that make Scrum work: the ability to inspect & adapt to changing circumstances. -->

これらの原則は深く相互にリンクしており、その中心にはスクラムを機能させる基本があります：変化する状況に対して検査し適応する能力です。

<!-- If the goal, from a technical perspective, is to support this ability to inspect & adapt, then clearly one should be able to detect and highlight (inspect) problems easily and quickly, and be able to change (adapt) the code to meet new circumstances, whatever they may be. To do this, people need to efficiently identify problems and, when they do, make changes to resolve them safely and easily. -->

技術的な観点からの目標がこの検査と適応の能力をサポートすることであるなら、明らかに問題を簡単かつ迅速に検出し強調（検査）できるべきであり、新しい状況がどのようなものであっても、それに対応するためにコードを変更（適応）できるべきです。これを行うために、人々は問題を効率的に特定し、特定したときには安全かつ簡単に変更を行って解決する必要があります。

<!-- An adaptive approach to [Modern Software Engineering](https://www.amazon.com/Modern-Software-Engineering-Discipline-Development/dp/0137314914/)[^1] is then built on two foundational assumptions: -->

[モダンソフトウェアエンジニアリング](https://www.amazon.com/Modern-Software-Engineering-Discipline-Development/dp/0137314914/)[^1]への適応的アプローチは、2つの基礎的な仮定の上に構築されています：

<!-- 1. that the discipline of software development is fundamentally a process of exploration and discovery, and
2. that the best way to facilitate such a process is by **Optimizing for Learning** and sustaining the ability to learn by **Optimizing to Manage Complexity**. -->

1. ソフトウェア開発の規律は根本的に探索と発見のプロセスであること、そして
2. そのようなプロセスを促進する最良の方法は、**学習の最適化**と**複雑性を管理するための最適化**によって学習能力を維持することです。

<!-- ## Core Practices -->

## コアプラクティス {#core-practices}

<!-- #### Optimizing for Learning -->

#### 学習の最適化 {#optimizing-for-learning}

<!-- We, as individuals, teams, and as organisations, need to be good at learning at multiple levels. Guesses about the nature of the products we create will likely be wrong, and there will be misunderstandings about what users want or need. Even if not, once users see the system, their wants and needs will change. -->

私たちは、個人として、チームとして、そして組織として、複数のレベルで学習することに長けている必要があります。私たちが作成するプロダクトの性質についての推測はおそらく間違っており、ユーザーが何を望んでいるか、何を必要としているかについて誤解があるでしょう。そうでなくても、ユーザーがシステムを見ると、彼らの望みとニーズは変わります。

<!-- Effective teams and organisations need to learn continuously from people using their systems; solutions may not work as expected, product ideas may not work, so some ideas and theories will need to be established and tested to see whether they address users' needs and goals. -->

効果的なチームと組織は、システムを使用する人々から継続的に学習する必要があります。解決策が期待通りに機能しない可能性があり、プロダクトのアイデアが機能しない可能性があるため、いくつかのアイデアと理論を確立し、それらがユーザーのニーズと目標に対処するかどうかをテストする必要があります。

<!-- The result of all this uncertainty is that effective software development needs to be flexible and adaptive. There are five core practices at the heart of an adaptive approach to engineering that enable the kind of learning and exploration needed to build and adapt systems that better meet the needs of users and other stakeholders. -->

このすべての不確実性の結果、効果的なソフトウェア開発は柔軟で適応的である必要があります。エンジニアリングへの適応的アプローチの中心には、ユーザーや他のステークホルダーのニーズによりよく応えるシステムを構築し適応させるために必要な学習と探索を可能にする5つのコアプラクティスがあります。

<!-- They are: -->

それらは：

<!-- 1. **Work Iteratively** - _Work in small steps and evaluate the effectiveness of decisions and choices after each small step._
2. **Optimize for Fast Feedback** - _Collect high-quality, accurate feedback on decisions and deliver it to the person best positioned to act on it._
3. **Work Incrementally** - _Complex systems never spring fully formed from the mind of some creator; they are the products of an incremental accretion of understanding and features, built over time. One organizes to support that process of accretion, maintaining and enhancing the ability to change the system quickly and easily._
4. **Adopt an Experimental Approach** - _Treat every change to process, product, or technology as an experiment. Work to control the variables to attempt to understand the results. Treat failure as an opportunity to learn._
5. **Be Pragmatic - Empirical Learning** - _Engineering is not the same as pure science or mathematics; it is not seeking perfection; it aims to solve practical problems with high-quality solutions. One should learn from the reality of the system, as well as from the theories of how it does, or should, work._ -->

1. **反復的に作業する** - _小さなステップで作業し、各小さなステップの後に意思決定と選択の有効性を評価する。_
2. **高速フィードバックのために最適化する** - _意思決定に関する高品質で正確なフィードバックを収集し、それに対処するのに最適な立場にいる人に届ける。_
3. **漸進的に作業する** - _複雑なシステムは、創造者の心から完全に形成されて出現することはない。それらは時間をかけて構築された理解と機能の漸進的な蓄積の産物である。その蓄積プロセスをサポートし、システムを迅速かつ容易に変更する能力を維持・強化するように組織化する。_
4. **実験的アプローチを採用する** - _プロセス、プロダクト、またはテクノロジーへのすべての変更を実験として扱う。結果を理解しようとするために変数を制御する作業をする。失敗を学習の機会として扱う。_
5. **実用的であれ - 経験的学習** - _エンジニアリングは純粋な科学や数学と同じではない。完璧を求めているのではなく、高品質な解決策で実際の問題を解決することを目指している。システムの現実から学ぶべきであり、それがどのように機能するか、または機能すべきかの理論からも学ぶべきである。_

<!-- #### Optimizing to Manage Complexity -->

#### 複雑性を管理するための最適化 {#optimizing-to-manage-complexity}

<!-- Software development operates in inherently complex environments, built on deep stacks of abstractions and technologies, where even simple systems are only a few steps away from significant challenges. This complexity is not inherently negative; it also creates hidden opportunities, technical advances, and new ways users derive value—but when left unmanaged, it becomes a primary reason organisations struggle to sustain effective ways of working. Humans have evolved effective strategies for coping with complexity, such as compartmentalisation, and successful approaches to software development deliberately apply such strategies to steer complexity toward learning, value, and better outcomes. -->

ソフトウェア開発は、抽象化と技術の深いスタックの上に構築された、本質的に複雑な環境で運用されており、単純なシステムでさえ重大な課題からわずか数ステップしか離れていません。この複雑性は本質的に悪いものではありません。それは隠された機会、技術的進歩、ユーザーが価値を得る新しい方法も生み出します—しかし管理されないままだと、組織が効果的な作業方法を維持するのに苦労する主な理由になります。人間はコンパートメント化などの複雑性に対処するための効果的な戦略を進化させてきており、ソフトウェア開発への成功したアプローチはそのような戦略を意図的に適用して複雑性を学習、価値、より良いアウトカムに向けて導きます。

<!-- In software, this is vital to avoid the disastrous end of so many failed systems - the 'Big Ball of Mud,' legacy systems that everyone is too afraid to change. The goal of effective software development is fundamentally different, and to support a sustainable approach, people need to retain the ability to modify the software. This is not about predicting the future of all possible uses, but about compartmentalizing the system so that one can change one part or facet without those changes forcing change elsewhere. -->

ソフトウェアにおいて、これは多くの失敗したシステムの悲惨な結末—誰もが変更を恐れる「巨大な泥だんご」、レガシーシステム—を避けるために不可欠です。効果的なソフトウェア開発の目標は根本的に異なり、持続可能なアプローチをサポートするために、人々はソフトウェアを変更する能力を保持する必要があります。これは将来のすべての可能な使用を予測することについてではなく、システムをコンパートメント化して、一部または一面を変更してもその変更が他の場所での変更を強制しないようにすることについてです。

<!-- Of course, that also means that one should be able to detect when changes are unsafe, which is firmly in the realm of "optimizing for learning". Managing the system's complexity is about making it easy and safe to change. Here are five practices to inform every design decision and help people build software that is easier to change. -->

もちろん、それは変更が安全でないときに検出できるべきであることも意味し、これは「学習のための最適化」の領域にしっかりと属しています。システムの複雑性を管理することは、変更を簡単かつ安全にすることについてです。すべての設計決定に情報を提供し、変更しやすいソフトウェアを構築するのに役立つ5つのプラクティスがあります。

<!-- 1. **Modularity** - _the degree to which a system's components may be separated and recombined, often with the benefit of flexibility and variety in use._[^2]
2. **Cohesion** - _the degree to which the elements inside a module belong together._[^3]
3. **Separation of Concerns** - _a design principle for separating a computer program into distinct sections such that each section addresses a separate concern._[^4]
4. **Abstraction** - _the process of removing physical, spatial, or temporal details or attributes in the study of objects or systems to focus attention on details of greater importance._[^5]
5. **Managed Coupling** - managing the degree of interdependence between software modules; a measure of how closely connected two routines or modules are; the strength of the relationships between modules.[^6] -->

1. **モジュール性** - _システムのコンポーネントが分離され再結合できる度合いで、しばしば使用における柔軟性と多様性の利点を伴う。_[^2]
2. **凝集度** - _モジュール内の要素がどれだけ一緒に属しているかの度合い。_[^3]
3. **関心の分離** - _コンピュータプログラムを別々のセクションに分離し、各セクションが別々の関心を扱うための設計原則。_[^4]
4. **抽象化** - _より重要な詳細に注意を集中させるために、オブジェクトやシステムの研究において物理的、空間的、または時間的な詳細や属性を除去するプロセス。_[^5]
5. **結合度の管理** - ソフトウェアモジュール間の相互依存の度合いを管理すること。2つのルーチンやモジュールがどれだけ密接に接続されているかの尺度。モジュール間の関係の強さ。[^6]

<!-- Unmanaged complexity is seen by many as the primary reason organizations abandon Scrum under delivery pressure. Make the failure mode explicit so leaders recognize themselves in it. -->

管理されていない複雑性は、多くの人によって、組織がデリバリーのプレッシャー下でスクラムを放棄する主な理由と見なされています。リーダーが自分自身をそこに認識できるように、失敗モードを明示的にしてください。

<!-- ## Putting the 'Core Practices' into Practice -->

## 「コアプラクティス」を実践に移す {#putting-the-core-practices-into-practice}

<!-- It is easy to read these ten ideas as so obvious and so generally accepted that they have become a kind of "motherhood and apple pie" that everyone agrees with, but in doing so, something important is missed. Most of today's software development isn't practiced this way, but most great software development **is**. One would expect this kind of result from a genuine "engineering" approach. In other disciplines, **'Engineering' is the stuff that works!**. -->

これら10のアイデアを、誰もが同意する「当たり前のこと」のように非常に明白で一般的に受け入れられているものとして読むのは簡単ですが、そうすることで何か重要なことが見落とされます。今日のソフトウェア開発のほとんどはこのように実践されていませんが、ほとんどの素晴らしいソフトウェア開発は**そうです**。本物の「エンジニアリング」アプローチからこのような結果を期待するでしょう。他の分野では、**「エンジニアリング」は機能するものです！**

<!-- ### Controlling the Variables with Small Steps -->

### 小さなステップで変数を制御する {#controlling-the-variables-with-small-steps}

<!-- One should focus on things that can be understood and controlled, and on how work might be organized to achieve desired outcomes more deliberately, right from the start. Guidelines are needed to help people do this before they have learned enough to fully understand solutions to issues not yet well understood. People need a way of working that allows them to continuously grow their understanding so they can adapt the work. Grow understanding and adapt solutions to match it, relying on knowledge and learning rather than wishful thinking about desired outcomes. -->

理解し制御できるものに焦点を当て、最初から望ましいアウトカムをより意図的に達成するために作業をどのように組織化できるかに焦点を当てるべきです。まだよく理解されていない問題の解決策を完全に理解するのに十分なことを学ぶ前に、人々がこれを行うのを助けるガイドラインが必要です。人々は、作業を適応させることができるように、理解を継続的に成長させることができる作業方法を必要としています。望ましいアウトカムについての希望的観測ではなく、知識と学習に頼って、理解を成長させ、それに合わせて解決策を適応させてください。

<!-- If engineers get this right, they can use this approach to explore the details of understood areas, moving them closer to desired outcomes with a lower risk of failure, while deferring other aspects of the system until they are ready to learn more about them. -->

エンジニアがこれを正しく行えば、このアプローチを使用して理解された領域の詳細を探索し、失敗のリスクを低くしながら望ましいアウトカムに近づけ、システムの他の側面についてもっと学ぶ準備ができるまで延期できます。

<!-- ### Progress via Incremental Change -->

### 漸進的変更による進歩 {#progress-via-incremental-change}

<!-- Treating learning as the core of discipline shifts the focus from relying on arbitrary predictions of the future, which are inherently wrong or at least imprecise, to a more deliberate, exploratory approach that defines how to make useful, dependable, incremental progress. -->

学習を規律の中核として扱うことで、焦点が本質的に間違っているか少なくとも不正確な未来の恣意的な予測に頼ることから、有用で信頼できる漸進的な進歩を達成する方法を定義する、より意図的で探索的なアプローチに移ります。

<!-- Some people trade off an illusion of precision in predicting the future, "We will deliver features x, y, and z by Q2 next year", for optimizing to work more efficiently to achieve great results more quickly. -->

一部の人々は、未来を予測する精度の幻想「来年第2四半期までに機能x、y、zを納品します」を、より効率的に作業して素晴らしい結果をより迅速に達成するための最適化と交換します。

<!-- ### Adopting a More Rational Approach -->

### より合理的なアプローチの採用 {#adopting-a-more-rational-approach}

<!-- To adopt a stronger **engineering-led approach** means being grounded in rationality and reality. Let's be clear: **trying to fix time, budget, and scope is irrational**; it won't work, and it provides a very poor basis for planning. -->

より強力な**エンジニアリング主導のアプローチ**を採用することは、合理性と現実に基づくことを意味します。明確にしましょう：**時間、予算、スコープを固定しようとすることは非合理的です**。それは機能せず、計画のための非常に貧弱な基盤を提供します。

<!-- When a specific delivery date matters, a generally reliable approach—where circumstances allow—is to keep the software continuously releasable. If advance communication is necessary, it can be helpful to remain deliberately flexible about the exact content of the release. At the time of writing, Apple exemplified this approach by avoiding detailed pre-announcements whenever possible. -->

特定の納品日が重要な場合、一般的に信頼できるアプローチは—状況が許す限り—ソフトウェアを継続的にリリース可能な状態に保つことです。事前のコミュニケーションが必要な場合、リリースの正確な内容について意図的に柔軟性を保つことが役立ちます。執筆時点では、Appleは可能な限り詳細な事前発表を避けることでこのアプローチを例示していました。

<!-- To deliver a fixed set of features, engineers should again work to ensure the system is always releasable, but remain vague about when to release it. Engineers can announce new features once they are in production and ready for release. Once again, some of the most successful companies in the world work to that model. -->

固定された機能セットを納品するために、エンジニアは再びシステムが常にリリース可能であることを確保するように作業すべきですが、いつリリースするかについては曖昧なままにすべきです。エンジニアは、新機能が本番環境にあり、リリースの準備ができたら発表できます。繰り返しますが、世界で最も成功している企業のいくつかはそのモデルで作業しています。

<!-- These strategies are more effective at achieving realistic goals than crossing your fingers and hoping for luck this time while attempting to fix both time and scope. -->

これらの戦略は、時間とスコープの両方を固定しようとしながら指を交差させて今回は運がいいことを願うよりも、現実的な目標を達成するのに効果的です。

<!-- ### Engineering Constraints - Guardrails to achieve better results -->

### エンジニアリング制約 - より良い結果を達成するためのガードレール {#engineering-constraints-guardrails-to-achieve-better-results}

<!-- The idea behind this list of ten practices is not to serve as gentle reminders of ideas we have all heard before, but to recommend them as tools to actively steer decision-making. If engineers consistently prioritize these factors in everything they do, they **will achieve better overall results**. -->

この10のプラクティスのリストの背後にあるアイデアは、私たちが以前に聞いたアイデアの穏やかなリマインダーとして機能することではなく、意思決定を積極的に導くためのツールとして推奨することです。エンジニアがこれらの要因を行うすべてのことで一貫して優先すれば、**より良い全体的な結果を達成します**。

<!-- This is not a model where people switch off their thinking and mechanically follow a set of steps. These are practices to adopt and apply intelligently. By default, people often choose options that maximize opportunities to learn, the ability to handle the complexity of the systems built, and the problems they are designed to address. -->

これは人々が思考を切って機械的に一連のステップに従うモデルではありません。これらは知的に採用し適用するプラクティスです。デフォルトでは、人々はしばしば学習の機会を最大化し、構築されたシステムの複雑性を処理する能力、およびそれらが対処するように設計された問題を最大化するオプションを選択します。

<!-- Maximizing feedback creates more opportunities to learn. If all feedback indicates "all is well", engineers can be more confident in the changes, make progress with greater certainty, faster, and with less stress. -->

フィードバックを最大化することで、学習の機会が増えます。すべてのフィードバックが「すべて順調」を示している場合、エンジニアは変更についてより自信を持ち、より確実に、より速く、ストレスを少なくして進歩できます。

<!-- Optimizing working practices, technology choices, and designs to deliver fast, high-quality feedback means engineers will necessarily need to make progress in smaller steps. -->

高速で高品質なフィードバックを提供するために作業プラクティス、技術の選択、設計を最適化することは、エンジニアが必然的により小さなステップで進歩する必要があることを意味します。

<!-- Smaller steps are safer, easier to test, easier to revert if something goes wrong, and make it easier to identify the cause of any failure and understand how to correct it. -->

より小さなステップはより安全で、テストがより容易で、何か問題が発生した場合に元に戻すことがより容易で、失敗の原因を特定し、それを修正する方法を理解することがより容易になります。

<!-- People will continue to optimize their work to gather clear, definitive feedback multiple times per day. At a minimum, engineers should **assess the software's releasability at least once per day**. -->

人々は1日に複数回、明確で決定的なフィードバックを収集するために作業を最適化し続けます。少なくとも、エンジニアは**1日に少なくとも1回、ソフトウェアのリリース可能性を評価すべきです**。

<!-- The ability to achieve this forces people to adopt other good behaviors and practices. -->

これを達成する能力は、人々に他の良い行動とプラクティスを採用することを強制します。

<!-- If engineers need fast, definitive feedback, they must verify that each small change is safe and sound, so they adopt the discipline of continuously verifying the releasability of the systems. But also, if they are going to make progress in this series of many small steps, and do that effectively at the lowest long-term costs (efficiently), they also need to be able to take those small steps easily and with minimum overhead. -->

エンジニアが高速で決定的なフィードバックを必要とする場合、各小さな変更が安全で健全であることを検証する必要があるため、システムのリリース可能性を継続的に検証する規律を採用します。しかし、この多くの小さなステップのシリーズで進歩し、最低の長期コスト（効率的に）でそれを効果的に行う場合、それらの小さなステップを簡単に最小限のオーバーヘッドで取ることができる必要もあります。

<!-- Engineers can't afford lengthy, messy bureaucracy; they need validation to be fast, reliable, and comprehensive. This leads people to adopt high levels of automation and to rely on it to determine the correctness and releasability of their systems. -->

エンジニアは長い、乱雑な官僚主義を許容できません。彼らは検証が速く、信頼性があり、包括的である必要があります。これにより、人々は高レベルの自動化を採用し、システムの正確性とリリース可能性を決定するためにそれに依存するようになります。

<!-- Automation can be complicated, but when done well, it reduces complexity. Many organizations have attempted to automate builds, tests, and deployments, only to struggle to do so effectively. Taking an engineering perspective helps people to do a better job of this. If engineers want the automated tests to be fast and effective, they need to actively **control variables** using version control, not just for source code but for every change to production. -->

自動化は複雑になる可能性がありますが、うまく行われると複雑性を減らします。多くの組織がビルド、テスト、デプロイメントを自動化しようとしましたが、効果的に行うのに苦労しました。エンジニアリングの視点を取ることで、人々はこれをより良く行うことができます。エンジニアが自動化テストを高速で効果的にしたい場合、ソースコードだけでなく、本番環境へのすべての変更にバージョン管理を使用して積極的に**変数を制御**する必要があります。

<!-- We adopt techniques such as **Infrastructure as Code** and policies such as **All Change to Production is Made via Version Control.** -->

私たちは**Infrastructure as Code**などの技術と、**本番環境へのすべての変更はバージョン管理を通じて行われる**などのポリシーを採用します。

<!-- Suppose engineers want small changes to be safe and good. In that case, they need it to be easy to determine safety and goodness, and for that, they need **Easily Testable Code** that has a significant impact on design choices, because designs that are easy to test also demand code that effectively **Handles Complexity**. -->

エンジニアが小さな変更を安全で良いものにしたい場合、安全性と良さを判断しやすくする必要があり、そのためには設計の選択に大きな影響を与える**テストしやすいコード**が必要です。テストしやすい設計は効果的に**複雑性を処理する**コードも要求するからです。

<!-- By intentionally aiming for code and designs that are easier to test, engineers significantly improve their ability to handle complexity consistently and sustainably. Writing tests before writing the code is an important aspect of this approach, but it does not fully capture its purpose. Test-Driven Development (TDD)—often more accurately described as Test-Driven Design—uses tests as a design tool. By applying early pressure to design decisions, TDD encourages simpler structures, clearer responsibilities, and better separation of concerns, thereby improving testability and increasing overall design quality. -->

テストしやすいコードと設計を意図的に目指すことで、エンジニアは複雑性を一貫して持続可能に処理する能力を大幅に向上させます。コードを書く前にテストを書くことはこのアプローチの重要な側面ですが、その目的を完全には捉えていません。テスト駆動開発（TDD）—しばしばテスト駆動設計とより正確に表現される—はテストを設計ツールとして使用します。設計決定に早期のプレッシャーを適用することで、TDDはよりシンプルな構造、より明確な責任、より良い関心の分離を奨励し、それによってテスト可能性を向上させ、全体的な設計品質を高めます。

<!-- The dependencies and interactions among the **ten** principles are more complex than this description suggests; it represents only one possible route through them, one chain of rational reasoning. Starting with Fast Feedback and Small Steps is a particularly effective way to frame the discussion, but the same case for a rational engineering approach could equally be made by beginning with Modularity, Working Experimentally, or Managing Coupling, and arriving at the same conclusions. -->

**10の**原則間の依存関係と相互作用は、この説明が示唆するよりも複雑です。それはそれらを通る可能な1つのルート、合理的な推論の1つの連鎖を表しているにすぎません。高速フィードバックと小さなステップから始めることは議論をフレーミングする特に効果的な方法ですが、合理的なエンジニアリングアプローチのための同じ議論は、モジュール性、実験的な作業、または結合度の管理から始めても同じ結論に到達できます。

<!-- All of these practices are very closely related to one another. This is a collection of deeply related fundamentals for discipline that, if used as a _**"North Star for decision making"**_, will lead people to better, more effective outcomes. In this case, see the North Star as lighting the path rather than the destination. -->

これらのプラクティスはすべて互いに非常に密接に関連しています。これは、_**「意思決定のための北極星」**_として使用すれば、人々をより良い、より効果的なアウトカムに導く、規律のための深く関連した基礎のコレクションです。この場合、北極星を目的地ではなく道を照らすものとして見てください。

<!-- Think for a moment about these two collections of ideas, imagine two software products, similar to a product that you are working on now. Now imagine a version of that product where there is: -->

これらの2つのアイデアのコレクションについて少し考えてみてください。今取り組んでいるプロダクトに似た2つのソフトウェアプロダクトを想像してください。今、そのプロダクトのバージョンを想像してください：

<!-- - **No Iteration** - _getting everything right the first time_
- **No Feedback** - _making perfect predictions of what the users will need and what will work to deliver that to them_
- **No Incrementalism** - _building everything in one step, and crossing our fingers that everything will work in the end. I imagine that there will be a fairly lengthy 'integration period' to try everything out_
- **No Experimentation** - _All of the assumptions, guesses, technology choices, and design decisions were perfect, untried, and correct the first time at the beginning of the effort._
- **No Emergent Learning** - _the guesses of what the users wanted, how hackers would attack the system, and how the world changes in the future were all perfect too, so there is never a need to change anything. It's about 'keeping promises.'_ -->

- **反復なし** - _最初からすべてを正しくする_
- **フィードバックなし** - _ユーザーが何を必要とし、それを提供するために何が機能するかの完璧な予測をする_
- **漸進主義なし** - _すべてを1ステップで構築し、最終的にすべてがうまくいくことを願って指を交差させる。すべてを試すためにかなり長い「統合期間」があると想像する_
- **実験なし** - _すべての仮定、推測、技術の選択、設計決定は、取り組みの最初から完璧で、試されておらず、最初から正しかった。_
- **創発的学習なし** - _ユーザーが何を望んでいたか、ハッカーがシステムをどのように攻撃するか、世界が将来どのように変化するかの推測もすべて完璧だったので、何かを変更する必要はない。それは「約束を守ること」についてである。_

<!-- Now, imagine a second product we have described here. -->

では、ここで説明した2番目のプロダクトを想像してください。

<!-- 1. **Iterative:** Engineers working in small iterative steps, always ensuring that there is a working, releasable product, even after minor changes.
2. **Continuous Learning:** We continuously gather feedback and learn from it, and
3. **Incremental - always meeting the Definition of Output Done:** build up the systems incrementally, small, verified, change, by small, verified, change.
4. **Controlled Experimentation**: This allows people to actively test their ideas; as they become more accustomed to it, they gain greater control and begin treating every change as a small, controlled experiment. One crucial practical engineering outcome of these small, controlled experiments is the creation of dependable, automated tests, a test harness.
5. **Emergent Learning:** Engineers become so used to working in small steps that they can handle any change - even changes that come from what the system "teaches" us in production and from user feedback. And that leads to an important lesson: it's better to change your plan than to stick to a promise that turned out to be a bad idea. -->

1. **反復的:** エンジニアは小さな反復的なステップで作業し、小さな変更の後でも常に動作する、リリース可能なプロダクトがあることを確保する。
2. **継続的学習:** 私たちは継続的にフィードバックを収集し、そこから学ぶ。
3. **漸進的 - 常にアウトプット完成の定義を満たす:** システムを漸進的に構築する。小さな、検証された変更の連続で。
4. **制御された実験:** これにより、人々は自分のアイデアを積極的にテストできる。それに慣れてくると、より大きな制御を獲得し、すべての変更を小さな制御された実験として扱い始める。これらの小さな制御された実験の重要な実践的エンジニアリング成果の1つは、信頼できる自動テスト、テストハーネスの作成である。
5. **創発的学習:** エンジニアは小さなステップで作業することに慣れ、どんな変更でも処理できるようになる—本番環境でシステムが私たちに「教える」ことやユーザーフィードバックからの変更さえも。そして、それは重要な教訓につながる：悪いアイデアであることが判明した約束に固執するよりも、計画を変更する方が良い。

<!-- Which product would you prefer to work on? Which do you think is most likely to be a success? Which do you think is likely to deliver value most quickly and efficiently? -->

どちらのプロダクトで作業したいですか？どちらが成功する可能性が最も高いと思いますか？どちらが最も迅速かつ効率的に価値を提供する可能性が高いと思いますか？

<!-- Now imagine another two products, in the first, engineers ignore all the advice about how to manage complexity, so: -->

さて、別の2つのプロダクトを想像してください。最初のプロダクトでは、エンジニアは複雑性を管理する方法についてのすべてのアドバイスを無視しています：

<!-- - **No Modularity** - _All the code is in one big, messy function._
- **No Cohesion** - _global variables everywhere and a mish-mash of code doing different jobs jumbled together._
- **No Separation of Concerns** - _Code to calculate tax, mixed in with code to paint buttons blue, alongside code to store data in the cloud. Change one, and you inevitably change them all._
- **No Abstraction** - _No obvious organizing principles that help you to answer the question 'where should I implement this change?'_
- **Coupling is Unmanaged** - _Which usually means 'coupling is high', so engineers can't change code in one place without forcing change elsewhere, maybe everywhere else._ -->

- **モジュール性なし** - _すべてのコードが1つの大きな乱雑な関数にある。_
- **凝集度なし** - _あらゆる場所にグローバル変数があり、異なる仕事をするコードが混ざり合っている。_
- **関心の分離なし** - _税金を計算するコードが、ボタンを青く塗るコードと混ざり、クラウドにデータを保存するコードと一緒になっている。1つを変更すると、必然的にすべてを変更することになる。_
- **抽象化なし** - _「この変更をどこに実装すべきか？」という質問に答えるのに役立つ明らかな組織原則がない。_
- **結合度が管理されていない** - _これは通常「結合度が高い」ことを意味し、エンジニアは1か所でコードを変更しても、他の場所、おそらく他のすべての場所で変更を強制せずにはいられない。_

<!-- This description is so common that we have a name for it: we call systems that look like this **a Big Ball of Mud**. Now imagine the opposite: the system is:... -->

この説明は非常に一般的なので、名前があります：このようなシステムを**巨大な泥だんご**と呼びます。今、反対を想像してください：システムは：...

<!-- 1. **Modular** - _A system divided up into small, discrete parts, each of which has a clear demarcation at its boundary, an "inside" and an "outside", so that it can keep secrets from interactions from "outside"._
2. **Cohesive** - _All components "inside" are related to the job they perform, and everything they need to do their job is present._
3. Has a strong **Separation of Concerns** - _Each of these pieces is focused on doing one thing and doing it well._
4. Using **Abstraction** to simplify conversations between parts - _Interactions from the "outside" via these clearly defined lines of demarcation that represent contracts with the outside world hide, or at least obscure, the internal workings of these parts._
5. **Manages Coupling** with a general preference for looser coupling. This means that a change in one place or module is less likely to be disconnected from changes in another, keeping these parts _more decoupled. When a particular solution requires tighter coupling, engineers can proceed with care and greater control._ -->

1. **モジュール式** - _小さな離散的な部分に分割されたシステムで、それぞれが境界に明確な境界線、「内側」と「外側」を持ち、「外側」からの相互作用から秘密を守ることができる。_
2. **凝集している** - _「内側」のすべてのコンポーネントは、それらが実行する仕事に関連しており、仕事をするために必要なものすべてが存在する。_
3. 強力な**関心の分離**を持つ - _これらの各部分は、1つのことをうまく行うことに集中している。_
4. 部分間の会話を簡素化するために**抽象化**を使用する - _外部世界との契約を表すこれらの明確に定義された境界線を通じた「外側」からの相互作用は、これらの部分の内部動作を隠す、または少なくとも不明瞭にする。_
5. 一般的により緩い結合を好みながら**結合度を管理する**。これは、1つの場所またはモジュールでの変更が別の場所での変更から切り離される可能性が低く、これらの部分を_より疎結合に保つことを意味する。特定の解決策がより密な結合を必要とする場合、エンジニアは注意を払い、より大きな制御で進めることができる。_

<!-- Which of these two options would be preferable to work on, and which would have the best chance of success, both now and in the long term? It is reasonable to assume that the second product would be preferred, even without any knowledge of the technology it uses, the nature of the problems it addresses, or other specific details. -->

これらの2つのオプションのうち、どちらが作業するのに好ましく、どちらが今も長期的にも成功の可能性が最も高いでしょうか？使用する技術、対処する問題の性質、その他の具体的な詳細の知識がなくても、2番目のプロダクトが好まれると仮定することは合理的です。

<!-- _**Imagine how much value could be created if you combined the approaches from both of the second product examples: Agile, grounded in sound software engineering practices.**_ -->

_**両方の2番目のプロダクト例からのアプローチを組み合わせたら、どれだけの価値が創造できるか想像してください：健全なソフトウェアエンジニアリングプラクティスに基づいたアジャイル。**_

<!-- These ten ideas are, in general, better than the alternatives. If engineers consistently prioritize these ten things and maximize them across every aspect of their work, they will often achieve better results than alternatives. -->

これらの10のアイデアは、一般的に、代替案よりも優れています。エンジニアがこれらの10のことを一貫して優先し、作業のあらゆる側面でそれらを最大化すれば、代替案よりも良い結果を達成することがよくあります。

<!-- Apply these ten ideas to how you...
- Organize Scrum Teams and collaborate with others
- Decompose problems or opportunities
- Plan product development
- Architect systems
- Build systems
- Verify releasability
- Sign-off
- Deploy and deliver software products to your users
- Do rework to attempt to attain desired outcomes
- _**or anything else...**_ -->

これらの10のアイデアを以下の方法に適用してください...
- スクラムチームを組織し、他者と協力する
- 問題や機会を分解する
- プロダクト開発を計画する
- システムをアーキテクトする
- システムを構築する
- リリース可能性を検証する
- サインオフする
- ユーザーにソフトウェアプロダクトをデプロイし納品する
- 望ましいアウトカムを達成しようとするためにやり直しを行う
- _**またはその他何でも...**_

<!-- For all of the above, always **Optimize for Learning.** And, always **Optimize to Handle Complexity.** -->

上記のすべてにおいて、常に**学習のために最適化してください。**そして、常に**複雑性を処理するために最適化してください。**

<!-- **If whatever engineers are doing does NOT build 'Better Software Faster' (ideally in a direction of travel), it doesn't count as 'Engineering' yet!** -->

**エンジニアが何をしていても「より良いソフトウェアをより速く」構築しない場合（理想的には進行方向に）、それはまだ「エンジニアリング」とはカウントされません！**

<!-- "Engineering" should work to improve the results; otherwise, the idea makes no real sense. -->

「エンジニアリング」は結果を改善するために機能すべきです。そうでなければ、そのアイデアには本当の意味がありません。

<!-- If what "engineers" are doing is not yet "engineering", then they should change something that will improve the ability to learn, enhance the handling of complexity, or both. If engineers do any of those things, they will be closer to a workable solution. Keep changing things so you continually improve at building **Better Software Faster** than before (ideally in a coherent direction of travel); that is what "Inspect & Adapt" is really for! Use both of the [DORA metrics](https://dora.dev/guides/dora-metrics-four-keys/)[^7], **Stability & Throughput,** to [measure progress](https://leanpub.com/measuringcontinuousdelivery)[^8]. -->

「エンジニア」がしていることがまだ「エンジニアリング」ではない場合、学習能力を向上させるか、複雑性の処理を強化するか、またはその両方を改善する何かを変更すべきです。エンジニアがこれらのいずれかを行えば、実行可能な解決策に近づきます。以前よりも**より良いソフトウェアをより速く**構築することで継続的に改善されるように物事を変え続けてください（理想的には一貫した進行方向に）。それが「検査と適応」の本当の目的です！[DORAメトリクス](https://dora.dev/guides/dora-metrics-four-keys/)[^7]の両方、**安定性とスループット**を使用して[進捗を測定してください](https://leanpub.com/measuringcontinuousdelivery)[^8]。

<!-- ## Behaviours that Help to Drive the Change -->

## 変化を推進するのに役立つ行動 {#behaviours-that-help-to-drive-the-change}

<!-- ### Continuous Quality -->

### 継続的品質 {#continuous-quality}

<!-- - [Test-Driven Development](https://courses.cd.training/courses/tdd-tutorial)[^9] and other [test-first](https://nkdagility.com/resources/test-first-development/)[^10] approaches.
- [Automated unit](https://en.wikipedia.org/wiki/Unit_testing)[^11], [Integration](https://en.wikipedia.org/wiki/Integration_testing)[^12], and [Acceptance Tests](https://courses.cd.training/courses/acceptance-testing-webinar)[^13].
- A Definition of Output Done that requires tested and working software capable of addressing the Definition of Outcome Done. -->

- [テスト駆動開発](https://courses.cd.training/courses/tdd-tutorial)[^9]およびその他の[テストファースト](https://nkdagility.com/resources/test-first-development/)[^10]アプローチ。
- [自動化されたユニット](https://en.wikipedia.org/wiki/Unit_testing)[^11]、[統合](https://en.wikipedia.org/wiki/Integration_testing)[^12]、および[受け入れテスト](https://courses.cd.training/courses/acceptance-testing-webinar)[^13]。
- アウトカム完成の定義に対処できる、テスト済みで動作するソフトウェアを要求するアウトプット完成の定義。

<!-- These behaviors, when combined, support learning and the ability to manage complexity. Test-Driven Development, gives fast iterative feedback on work, but also supplies a forcing-function that guides design in better directions, encouraging the creation of more modular, cohesive, better abstracted, more loosely-coupled systems with better separation of concerns, because systems like that are more easily testable. -->

これらの行動は、組み合わされると、学習と複雑性を管理する能力をサポートします。テスト駆動開発は、作業に対する高速な反復フィードバックを提供しますが、設計をより良い方向に導く強制機能も提供し、より良い関心の分離を持つ、よりモジュール式で、凝集度が高く、より良く抽象化され、より疎結合なシステムの作成を奨励します。そのようなシステムはより簡単にテストできるからです。

<!-- Working to establish, and vitally, maintain, **high-quality and desired outcomes is fundamental to any successful approach**. Delivering "rubbish" faster does not promote adaptiveness. If engineers can reliably and repeatedly deliver a high-quality product, they can confidently proceed in small, safe steps. -->

**高品質で望ましいアウトカムを確立し、そして重要なことに維持することは、成功するあらゆるアプローチの基本です**。「ゴミ」をより速く納品することは適応性を促進しません。エンジニアが信頼性を持って繰り返し高品質のプロダクトを納品できれば、自信を持って小さな安全なステップで進むことができます。

<!-- For this, engineers need fast, timely feedback on their work, and for that, they need fast, repeatable test results so that small, safe (sometimes parallel) steps help build confidence in their work and provide evidence of success. -->

このために、エンジニアは作業に対する高速でタイムリーなフィードバックが必要であり、そのためには高速で再現可能なテスト結果が必要です。それにより、小さな安全な（時には並行した）ステップが作業への信頼を構築し、成功のエビデンスを提供するのに役立ちます。

<!-- Good automated testing is central to a sound engineering approach, providing a form of "measurement" that determines the correctness of systems, and, in turn, leads to [better-designed systems](https://youtu.be/ln4WnxX-wrw)[^14]. -->

優れた自動テストは健全なエンジニアリングアプローチの中心であり、システムの正確性を決定する「測定」の形式を提供し、それが[より良く設計されたシステム](https://youtu.be/ln4WnxX-wrw)[^14]につながります。

<!-- Testable systems are **better systems**: -->

テスト可能なシステムは**より良いシステム**です：

<!-- - More modular so that engineers can focus testing on smaller and simpler pieces.
- More cohesive so that engineers can better control the variables within the scope of a test, and so get more determinate results.
- Have better separation of concerns so engineers can test each system behavior in isolation, making tests simpler and more focused on the problem at hand.
- Good tests test behavioural outcomes rather than internal implementation details. So, engineers have clear lines of abstraction to separate system components, allowing them to evaluate what they do without over-testing implementation details in place. This means engineers can change the implementation without invalidating the test.
- Good tests act as specifications of the intent, rather than "after the fact" assertions that the code works. This often works best when engineers write the test before the code, which helps ensure tests are easy to write. If the test is difficult to write, or many tests are needed for a single piece of code, it indicates a poor design. Product Developers can change the external design of the code and systems to make them more testable, thereby increasing abstraction and reducing coupling, almost as a side effect. It's often helpful to treat TDD as test-driven design. -->

- よりモジュール式であるため、エンジニアはより小さくシンプルな部分にテストを集中できます。
- より凝集度が高いため、エンジニアはテストの範囲内で変数をより良く制御でき、より決定的な結果を得ることができます。
- より良い関心の分離があるため、エンジニアは各システムの振る舞いを分離してテストでき、テストがよりシンプルで手元の問題により集中したものになります。
- 優れたテストは内部実装の詳細ではなく振る舞いのアウトカムをテストします。したがって、エンジニアはシステムコンポーネントを分離する明確な抽象化の線を持ち、実装の詳細を過度にテストすることなく、それらが何をするかを評価できます。これはエンジニアがテストを無効にすることなく実装を変更できることを意味します。
- 優れたテストは、コードが機能するという「事後の」アサーションではなく、意図の仕様として機能します。これはエンジニアがコードの前にテストを書くときに最もうまく機能することが多く、テストが書きやすいことを保証するのに役立ちます。テストを書くのが難しい場合、または単一のコードに多くのテストが必要な場合、それは設計が悪いことを示しています。プロダクト開発者はコードとシステムの外部設計を変更してそれらをよりテスト可能にし、それによって副作用としてほとんど抽象化を増やし結合を減らすことができます。TDDをテスト駆動設計として扱うことがしばしば役立ちます。

<!-- In summary, testable systems must be tested early and throughout the development process, not after implementation is complete. Waiting for a system to be deemed complete is missing the most significant value of testing in software development, which is to use it as a form of measurement of the correctness of our work. In this, more engineering-focused approach, automated testing is the equivalent of a carpenter using a ruler to decide where to cut the wood. Our testing steers our design decisions, and this is how we achieve better results. -->

要約すると、テスト可能なシステムは、実装が完了した後ではなく、開発プロセスの早い段階で、そして全体を通じてテストされなければなりません。システムが完成したとみなされるのを待つことは、ソフトウェア開発におけるテストの最も重要な価値、つまり作業の正確性の測定の形式としてそれを使用することを見逃しています。この、よりエンジニアリングに焦点を当てたアプローチでは、自動テストは大工が木を切る場所を決めるために定規を使うのと同等です。私たちのテストは設計決定を導き、これが私たちがより良い結果を達成する方法です。

<!-- ### Continuous Integration and Delivery -->

### 継続的インテグレーションとデリバリー {#continuous-integration-and-delivery}

<!-- - Integrating into the main [branch](https://en.wikipedia.org/wiki/Version_control)[^15] frequently, at least once a day.
- Automated build and [deployment pipelines](https://youtu.be/m1oMj29P--Y)[^16].
- Test environments that closely mirror production. -->

- メイン[ブランチ](https://en.wikipedia.org/wiki/Version_control)[^15]に頻繁に、少なくとも1日1回統合する。
- 自動化されたビルドと[デプロイメントパイプライン](https://youtu.be/m1oMj29P--Y)[^16]。
- 本番環境に近いテスト環境。

<!-- #### Continuous Integration -->

#### 継続的インテグレーション {#continuous-integration}

<!-- Continuous Integration (CI) is not about tools; it is about a [better way of working](https://youtu.be/NcU0oEk6z8Y)[^17]. If you think about two or more copies of the same code being worked on and modified in parallel, this represents a messy state to be in. Which one is "correct"? Maybe even more important, what is the current **truth of the system**? -->

継続的インテグレーション（CI）はツールについてではありません。それは[より良い作業方法](https://youtu.be/NcU0oEk6z8Y)[^17]についてです。同じコードの2つ以上のコピーが並行して作業され修正されていることを考えると、これは乱雑な状態を表しています。どれが「正しい」のでしょうか？おそらくさらに重要なのは、**システムの現在の真実**は何かということです。

<!-- There is no way to definitively answer either question until engineers merge the two copies and resolve any issues they identify. Only then can they tell that the changes work together. This point of merging changes is how engineers establish a definitive **shared truth for the system**. CI focuses on [increasing the frequency with which changes are merged](https://youtu.be/lXQEi1O5IOI)[^18] to make such a valuation and gain insight into the correctness, or otherwise, of the system. -->

エンジニアが2つのコピーをマージし、特定した問題を解決するまで、どちらの質問にも決定的に答える方法はありません。その時初めて、変更が一緒に機能することを伝えることができます。この変更をマージするポイントは、エンジニアが**システムの共有された決定的な真実**を確立する方法です。CIは[変更がマージされる頻度を増やすこと](https://youtu.be/lXQEi1O5IOI)[^18]に焦点を当てて、そのような評価を行い、システムの正確性またはその他の洞察を得ます。

<!-- The definition of CI is:
_**Continuous Integration is a software development practice where each member of a team merges their changes into a codebase together with their colleagues' changes at least daily. Each of these integrations is verified by an automated build (including test) to detect integration errors as quickly as possible. Teams find that this approach reduces the risk of delivery delays, reduces the effort of integration, and enables practices that foster a healthy codebase for rapid enhancement with new features[^35].**_
_**– Martin Fowler**_ -->

CIの定義は：
_**継続的インテグレーションは、チームの各メンバーが少なくとも毎日、同僚の変更と一緒にコードベースに自分の変更をマージするソフトウェア開発プラクティスです。これらの各統合は、統合エラーをできるだけ早く検出するために自動化されたビルド（テストを含む）によって検証されます。チームは、このアプローチが納品遅延のリスクを減らし、統合の労力を減らし、新機能による迅速な拡張のための健全なコードベースを育成するプラクティスを可能にすることを発見しています[^35]。**_
_**– Martin Fowler**_

<!-- In short, everyone working in a shared codebase commits their changes to a shared version of the truth at least once per day, and that snapshot is evaluated for correctness. -->

要するに、共有コードベースで作業するすべての人が、少なくとも1日1回、真実の共有バージョンに自分の変更をコミットし、そのスナップショットが正確性について評価されます。

<!-- After every commit, engineers definitively establish a new snapshot of the **Truth** - the "Current State of the System". -->

すべてのコミットの後、エンジニアは**真実**—「システムの現在の状態」—の新しいスナップショットを決定的に確立します。

<!-- This serves as a synchronisation point, often eliminating ambiguity. Changes to this "Current State" are made sequentially and under strict version control, so they always represent a definitive, accurate, reproducible record of the system. -->

これは同期ポイントとして機能し、しばしば曖昧さを排除します。この「現在の状態」への変更は順番に、厳格なバージョン管理の下で行われるため、常にシステムの決定的で正確で再現可能な記録を表します。

<!-- To qualify as "Continuous" Integration, everyone should **Commit Changes to CI at Least Once per Day**. This is the minimum frequency of "commit" required to count as "Continuous". -->

「継続的」インテグレーションとして認定されるには、全員が**少なくとも1日1回CIに変更をコミットすべきです**。これは「継続的」としてカウントされるために必要な「コミット」の最小頻度です。

<!-- Without this daily sharing, engineers risk losing visibility into the system's current state and, as a result, face many problems. CI is the closest engineers can get to a definitive, clear view of the system's state; anything else is, by definition, less certain and therefore more risky. The DORA data show that teams that merge their changes at least daily produce significantly higher-quality systems, more quickly, than teams that don't. CI is the route to **Better Software Faster**. -->

この毎日の共有がなければ、エンジニアはシステムの現在の状態への可視性を失うリスクがあり、その結果、多くの問題に直面します。CIはエンジニアがシステムの状態の決定的で明確なビューに最も近づくことができる方法です。他のものは、定義上、より不確実であり、したがってよりリスクが高いです。DORAデータは、少なくとも毎日変更をマージするチームが、そうでないチームよりも大幅に高品質のシステムをより迅速に生産することを示しています。CIは**より良いソフトウェアをより速く**への道です。

<!-- The DORA group at Google initiated the most scientifically credible research on software development practices... -->

GoogleのDORAグループは、ソフトウェア開発プラクティスに関する最も科学的に信頼性の高い研究を何年にもわたって開始し、何万ものアンケートで構成されています。彼らは社会学へのピアレビューされたアプローチとデータの強力な統計分析を使用し、ソフトウェア開発プラクティスとより良いアウトカムの間のパターンと関係を強調する経験的に根拠のあるモデルを構築しました。以下の測定に基づいています：

- **安定性** - エンジニアが構築するシステムの品質
- **スループット** - エンジニアがその品質の変更を提供できる速度

_この研究の背後にある科学とその重要な発見のいくつかについては、Nichole Forsgren、Jez Humble、Gene Kimによる書籍「Accelerate」をお読みください[^36]_

<!-- The problem with CI is that it demands some trade-offs... -->

CIの問題は、いくつかのトレードオフを要求することです。エンジニアが迅速、安全、効率的に作業できるようにするための十分なフィードバックを得るために少なくとも毎日変更をコミットする**必要がある**場合、これはエンジニアが**「コミット」**の性質について考える方法を変えます。CIでは、「変更をコミットする」とは、「この変更が機能することを意図していることにコミットした」ことを意味します。これを継続的デリバリー（以下で説明するCD）の定義に拡張すると、「この変更が本番環境の準備ができていることにコミットしている」ことになります。

<!-- There are a variety of ways to achieve this CI way of working, including: -->

このCI方式の作業を達成するためのさまざまな方法があります：

- [ダークローンチング](https://martinfowler.com/bliki/DarkLaunching.html)[^19] - _部分的に完成した機能を、使用の準備ができるまでユーザーに見えるルートを提供しないことで隠す_
- [抽象化によるブランチ](https://martinfowler.com/bliki/BranchByAbstraction.html)[^20] - 変更しようとしているコードを抽象化の後ろに分離するように既存のコードをリファクタリングし、_新しい抽象化を使用して_古いコードの代替品を開発することで機能する
- [フィーチャーフラグ](https://martinfowler.com/bliki/FeatureFlag.html)[^21] - _人々がユーザーがどのバージョンの機能と相互作用するかを選択できるソフトウェアスイッチ_

<!-- Fundamentally, the objective of working this way is to separate the acts of deploying change into production from the decision to release new features to users. -->

根本的に、この方法で作業する目的は、本番環境に変更をデプロイする行為を、ユーザーに新機能をリリースする決定から分離することです。

**デプロイの決定はリリースの決定から分離されます。**

<!-- In a Scrum Team, the Developers work to ensure that their system is always ready to deploy, while the decision to release may be influenced by other, non-technical considerations. -->

スクラムチームでは、開発者はシステムが常にデプロイの準備ができていることを確保するように作業し、一方でリリースの決定は他の非技術的な考慮事項によって影響を受ける可能性があります。

<!-- #### Continuous Delivery -->

#### 継続的デリバリー {#continuous-delivery}

<!-- [Continuous Delivery](https://courses.cd.training/courses/cd-fundamentals)[^22] is CI's big brother; if CI is about continuously validating that the changes are working together, CD "ups the ante": -->

[継続的デリバリー](https://courses.cd.training/courses/cd-fundamentals)[^22]はCIの兄貴分です。CIが変更が一緒に機能していることを継続的に検証することについてであるなら、CDは「賭け金を上げます」：

**継続的デリバリー：ソフトウェアを常にリリース可能な状態に保つこと。**

<!-- The idea is to establish the system as a releasable thing from the outset: it is designed, developed, packaged, and tested to production quality, so it can be released to production without further work. We then maintain it in that state for the rest of its life. -->

アイデアは、最初からシステムをリリース可能なものとして確立することです：それは設計され、開発され、パッケージ化され、本番品質でテストされるため、追加の作業なしで本番環境にリリースできます。そして、その残りの寿命の間、その状態を維持します。

<!-- To do that, we need to version-control and automate everything we can: functional testing, unit testing, performance testing, security testing, configuration management, deployment, data migration, regulatory compliance, etc. -->

そのために、できるすべてのものをバージョン管理し自動化する必要があります：機能テスト、ユニットテスト、パフォーマンステスト、セキュリティテスト、構成管理、デプロイメント、データ移行、規制コンプライアンスなど。

<!-- The goal is to automate every check that determines whether the system is releasable - build, tests, security checks, quality rules, and deployment steps. -->

目標は、システムがリリース可能かどうかを決定するすべてのチェックを自動化することです—ビルド、テスト、セキュリティチェック、品質ルール、デプロイメントステップ。

<!-- We bundle those automated checks into a [Deployment Pipeline](https://youtu.be/eoaDr5PpT2c)[^24]. It's not just a build script; it's an end-to-end process that asserts whether, or not, a change is safe to release. -->

これらの自動化されたチェックを[デプロイメントパイプライン](https://youtu.be/eoaDr5PpT2c)[^24]にバンドルします。それは単なるビルドスクリプトではありません。変更がリリースしても安全かどうかを主張するエンドツーエンドのプロセスです。

**1つのテストが失敗したら、変更を拒否します！**

<!-- #### Continuous Deployment -->

#### 継続的デプロイメント {#continuous-deployment}

**継続的デプロイメント** - _**成功した変更のたびに、自動的に本番環境に変更をプッシュする**_

<!-- **Releasing frequently is generally less risky than releasing infrequently**. -->

**頻繁にリリースすることは、一般的に頻繁にリリースしないよりもリスクが低いです**。各変更が小さい場合、本質的によりシンプルです。つまり、間違いが隠れる場所が少なくなります。各変更が小さい場合、より簡単にテストでき、間違っていても、より簡単に元に戻すことができます。

DORAの調査データに基づいて、この頻繁で小さな検証された変更のシーケンスで作業するモデルは、**安定性とスループット**の高スコアの大幅に強力な予測因子です。つまり、これらのスクラムチームが**より良いソフトウェアをより速く**生産することを意味するスコアです。DORA研究のより深い発見の1つは、「**スピードと品質の間にトレードオフはない**」ということです。

<!-- ### Design and Architecture for Adaptability -->

### 適応性のための設計とアーキテクチャ {#design-and-architecture-for-adaptability}

- [コンテキスト](https://youtu.be/wQYRl--58zM)[^31] - 誰がシステムを使用するか、どのように使用するか、将来どのように発展することを期待するかを理解することを学ぶ。
- [実験](https://youtu.be/wQYRl--58zM)[^31] - 文脈的理解を使用して、より多くの情報が役立つ場所を特定し、小さな制御された実験を使用してその情報を収集する。
- 設計を改善するための継続的な[リファクタリング](https://courses.cd.training/courses/refactoring-tutorial)[^30]。
- フィードバックによって導かれる[進化的アーキテクチャ](https://youtu.be/ElMnHDSFaCw)[^32]。
- [ペアまたはアンサンブルプログラミング](https://youtu.be/fbxMV76e7_E)[^33]などのコラボレーティブ設計技法。

<!-- If the goal is to maintain the software in an always-releasable state... -->

目標がソフトウェアを常にリリース可能な状態に維持することである場合、哲学的に最良の出発点は、私たちのアイデアは常に間違っている可能性があると仮定することであり、したがって、間違っている場所を特定し、物事をより良く行う方法、プロダクトのより良いアイデア、または質問へのより良い答えを見つけたときにそれらを修正できる必要があります。現実的には、システムを常に変更しやすくするように作業することによってのみ、これらのことを達成できます。

<!-- Making change easy is central to the CD approach. -->

変更を容易にすることはCDアプローチの中心です。「CDのための理想的なアーキテクチャ」は単一のものではありませんが、特定のアーキテクチャアプローチと選択はそれをより困難にする可能性があります。

根本的に、多くの小さな、安全な、検証された変更を通じて進歩するこのエンジニアリング駆動のアプローチは、人々にソフトウェア[設計](https://youtu.be/8GONv6jJsG0)[^31]と[アーキテクチャ](https://youtu.be/ElMnHDSFaCw)[^32]へのより進化的なアプローチを採用することを強制します。

<!-- ### Code Quality, Maintainability, and Cost -->

### コード品質、保守性、コスト {#code-quality-maintainability-and-cost}

- コードの集団的所有権と品質への責任。
- ペアリング、モビング、または構造化されたコードレビューを通じたピアレビュー。
- クリーンコードプラクティスと自動化された分析ツール。

**ソフトウェアシステムの品質は、変更がどれだけ容易かによって定義されます！**

これは重要です。なぜなら、ソフトウェア開発コストを大幅に削減するからです。高品質のソフトウェアを生産するにはコストがかかるという仮定がありますが、DORAのデータは反対のことを言っています。高品質を望むなら、より速く（より小さなステップで）動く必要があります。速く動きたいなら、より高品質の作業を生産する必要があります。

**「変更の容易さ」**は品質の奇妙な定義のように見えるかもしれませんが、実際には、私たちが価値を置く他のすべてのものの基礎にあり、媒体としてのソフトウェアの独自の強みを活用しています。変更の容易さがソフトウェアを「ソフト」にするものです。

<!-- ### Operational Excellence -->

### 運用エクセレンス {#operational-excellence}

- [モニタリング、オブザーバビリティ、実行中のシステムからの高速フィードバック](https://youtu.be/Nmu4URA7pSM)[^34]（しばしばテレメトリと呼ばれる）。
- フィーチャートグル、カナリアリリース、ダークローンチなどの技術。
- 自動ロールバックやカオステストなど、レジリエンスを構築するプラクティス。

<!-- #### Measuring Success through Observability -->

#### オブザーバビリティを通じた成功の測定 {#measuring-success-through-observability}

変更を容易にするために、私たちは人々が継続的に共有理解を構築し、学習文化とプロセスの基盤を築くのに役立つフィードバックループを確立し最適化することを目指しています。

良いソフトウェアを構築することが目的である場合に学ぶ必要がある最も重要な教訓は、ユーザーがそれをどう思うかです。そのために、本番環境を通じてフィードバックループを閉じる方法を見つける必要があります。

<!-- #### Continuous Releasability -->

#### 継続的リリース可能性 {#continuous-releasability}

継続的デリバリーの作業定義は、ソフトウェアが常にリリース可能な状態に保たれるということです。これは成功の重要な一般的な指標であり、単なる頻繁なリリースよりもプラクティスにとってより基本的です。

頻繁なリリースは非常に良いアイデアであり、多くのことを簡素化しますが、ビジネスの文脈、構築されているソフトウェアの性質、その他の要因にもより依存しています。アドバイスは、外部の文脈が許す限り頻繁にリリースすることです。

実際の目標は**より良いソフトウェアをより速く構築すること**です。頻繁なリリースはそれを達成するのに役立つ技術です。

_**ソフトウェアが常にリリース可能な状態になるように作業してください！**_

<!-- ## Conclusion -->

## 結論 {#conclusion}

<!-- This document is an overdue integration with the Scrum Guide Expansion Pack, as engineering practices are expressed in the 'Definition of Output Done' and they: -->

この文書は、エンジニアリングプラクティスが「アウトプット完成の定義」で表現され、以下を行うため、Scrum Guide Expansion Packとの待望の統合です：

<!-- - Enable each Sprint to produce a usable, potentially releasable Increment.
- Strengthen Scrum's pillars: Transparency (quality visible), Inspection (rapid feedback), and Adaptation (safe change).
- Reinforce the Scrum Values: Commitment to quality, Focus on working software, Openness about problems, Respect for users and Product Developers, Courage to improve practices. -->

- 各スプリントが使用可能で、潜在的にリリース可能なインクリメントを生産することを可能にする。
- スクラムの柱を強化する：透明性（品質が可視）、検査（迅速なフィードバック）、適応（安全な変更）。
- スクラムの価値を強化する：品質へのコミットメント、動作するソフトウェアへの集中、問題についてのオープンさ、ユーザーとプロダクト開発者への尊敬、プラクティスを改善する勇気。

<!-- These practices are well aligned with the core philosophies that underpin Scrum and strongly reinforce its effectiveness. Organizations that claim to 'do Scrum' without enabling these practices for engineering-oriented 'Scrum Teams' are running timeboxed project management under the guise of agile language, not the essence of Scrum. -->

これらのプラクティスは、スクラムを支える核心的な哲学とよく整合しており、その有効性を強く強化します。エンジニアリング指向の「スクラムチーム」に対してこれらのプラクティスを有効にせずに「スクラムをやっている」と主張する組織は、スクラムの本質ではなく、アジャイル言語を装ったタイムボックス化されたプロジェクト管理を実行しています。

<!-- Scrum Teams are responsible for choosing and applying engineering practices by defining and fulfilling an appropriate Definition of Done for their domain. It is inherent to Scrum and adaptive practices that improvement is ongoing. The engineering principles described here are the most evidenced version of what really works in practice in a very wide variety of different organizations, building different kinds of software from safety critical systems, through to high performance finance systems, global scale internet systems, banks, space craft, embedded systems, cars, military systems and in large scale enterprises, startups, legacy systems, and Scrum Teams building AAA Games. -->

スクラムチームは、自分たちのドメインに適切な完成の定義を定義し履行することで、エンジニアリングプラクティスを選択し適用する責任があります。改善が継続的であることは、スクラムと適応的プラクティスに固有のものです。ここで説明されているエンジニアリング原則は、安全クリティカルなシステムから高性能金融システム、グローバル規模のインターネットシステム、銀行、宇宙船、組み込みシステム、自動車、軍事システム、そして大規模企業、スタートアップ、レガシーシステム、AAAゲームを構築するスクラムチームに至るまで、非常に幅広いさまざまな組織で実際に機能するものの最もエビデンスに基づいたバージョンです。

<!-- Scrum Teams have successfully applied these techniques across all types of software and companies. These ideas are generic and work effectively wherever they are applied. If followed, they can help ensure success; while nothing guarantees results, one can be more confident that better outcomes will be achieved than if one does not do these things. After all, that's what "engineering" is really for! -->

スクラムチームはあらゆるタイプのソフトウェアと企業でこれらの技術を成功裏に適用してきました。これらのアイデアは汎用的であり、適用される場所ならどこでも効果的に機能します。従えば、成功を保証するのに役立ちます。結果を保証するものは何もありませんが、これらのことを行わない場合よりも、より良いアウトカムが達成されると確信できます。結局のところ、それが「エンジニアリング」の本当の目的です！

<!-- ## References -->

## 参考文献 {#references}

[^1]: Farley, D. (2021) _Modern Software Engineering: Doing What Works to Build Better Software Faster_. Addison-Wesley Professional. Available at: [https://www.amazon.com/Modern-Software-Engineering-Discipline-Development/dp/0137314914/](https://www.amazon.com/Modern-Software-Engineering-Discipline-Development/dp/0137314914/) (Accessed: 22 November 2025).

[^2]: Wikipedia (2023) 'Modularity'. _Wikipedia_. Available at: [https://en.wikipedia.org/wiki/Modularity](https://en.wikipedia.org/wiki/Modularity) (Accessed: 23 November 2025).

[^3]: Wikipedia (2023) 'Cohesion (computer science)'. _Wikipedia_. Available at: [https://en.wikipedia.org/wiki/Cohesion_(computer_science)](https://en.wikipedia.org/wiki/Cohesion_(computer_science)) (Accessed: 23 November 2025).

[^4]: Wikipedia (2023) 'Separation of concerns'. _Wikipedia_. Available at: [https://en.wikipedia.org/wiki/Separation_of_concerns](https://en.wikipedia.org/wiki/Separation_of_concerns) (Accessed: 23 November 2025).

[^5]: Wikipedia (2023) 'Abstraction (computer science)'. _Wikipedia_. Available at: [https://en.wikipedia.org/wiki/Abstraction_(computer_science)](https://en.wikipedia.org/wiki/Abstraction_(computer_science)) (Accessed: 23 November 2025).

[^6]: Wikipedia (2023) 'Coupling (computer programming)'. _Wikipedia_. Available at: [https://en.wikipedia.org/wiki/Coupling_(computer_programming)](https://en.wikipedia.org/wiki/Coupling_(computer_programming)) (Accessed: 23 November 2025).

[^7]: Harvey, N. (2025) 'DORA's software delivery metrics: the four keys'. _DORA_. Available at: [https://dora.dev/guides/dora-metrics-four-keys/](https://dora.dev/guides/dora-metrics-four-keys/) (Accessed: 22 November 2025).

[^8]: Smith, S. (2016) _Measuring Continuous Delivery_. Leanpub. Available at: [https://leanpub.com/measuringcontinuousdelivery](https://leanpub.com/measuringcontinuousdelivery) (Accessed: 22 November 2025).

[^9]: Farley, D. (2025) 'TDD Tutorial'. _CD.Training_. Available at: [https://courses.cd.training/courses/tdd-tutorial](https://courses.cd.training/courses/tdd-tutorial) (Accessed: 22 November 2025).

[^10]: Naked Agility with Martin Hinshelwood (no date) 'Test First Development'. Available at: [https://nkdagility.com/resources/test-first-development/](https://nkdagility.com/resources/test-first-development/) (Accessed: 23 November 2025).

[^11]: Wikipedia (2023) 'Unit testing'. _Wikipedia_. Available at: [https://en.wikipedia.org/wiki/Unit_testing](https://en.wikipedia.org/wiki/Unit_testing) (Accessed: 23 November 2025).

[^12]: Wikipedia (2023) 'Integration testing'. _Wikipedia_. Available at: [https://en.wikipedia.org/wiki/Integration_testing](https://en.wikipedia.org/wiki/Integration_testing) (Accessed: 23 November 2025).

[^13]: Farley, D. (2025) 'Acceptance Testing – Webinar'. _CD.Training_. Available at: [https://courses.cd.training/courses/acceptance-testing-webinar](https://courses.cd.training/courses/acceptance-testing-webinar) (Accessed: 22 November 2025).

[^14]: Farley, D. (2022) 'TDD Is the Best Design Technique'. _YouTube_. Available at: [https://youtu.be/In4WnXx-wrw](https://youtu.be/In4WnXx-wrw) (Accessed: 22 November 2025).

[^15]: Wikipedia (2023) 'Version control'. _Wikipedia_. Available at: [https://en.wikipedia.org/wiki/Version_control](https://en.wikipedia.org/wiki/Version_control) (Accessed: 23 November 2025).

[^16]: Farley, D. (2025) '3 Reasons Your CI/CD Pipeline Isn't Working As It Should…'. _YouTube_. Available at: [https://youtu.be/m1oMj29P--Y](https://youtu.be/m1oMj29P--Y) (Accessed: 22 November 2025).

[^17]: Farley, D. (2025) 'The 10 Commandments of Continuous Integration (CI)'. _YouTube_. Available at: [https://youtu.be/NcU0oEk6z8Y](https://youtu.be/NcU0oEk6z8Y) (Accessed: 22 November 2025).

[^18]: Farley, D. (2021) 'Why CI Is Better Than Feature Branching'. _YouTube_. Available at: [https://youtu.be/lXQEi1O5IOI](https://youtu.be/lXQEi1O5IOI) (Accessed: 22 November 2025).

[^19]: Fowler, M. (2020) 'Dark Launching'. _Martin Fowler_. Available at: [https://martinfowler.com/bliki/DarkLaunching.html](https://martinfowler.com/bliki/DarkLaunching.html) (Accessed: 22 November 2025).

[^20]: Fowler, M. (2014) 'Branch by Abstraction'. _Martin Fowler_. Available at: [https://martinfowler.com/bliki/BranchByAbstraction.html](https://martinfowler.com/bliki/BranchByAbstraction.html) (Accessed: 22 November 2025).

[^21]: Fowler, M. (2010) 'Feature Flag'. _Martin Fowler_. Available at: [https://martinfowler.com/bliki/FeatureFlag.html](https://martinfowler.com/bliki/FeatureFlag.html) (Accessed: 22 November 2025).

[^22]: CD Training (no date) _Continuous Delivery Fundamentals_. Available at: [https://courses.cd.training/courses/cd-fundamentals](https://courses.cd.training/courses/cd-fundamentals) (Accessed: 22 November 2025).

[^24]: Farley, D. (2020) _Continuous Delivery Pipelines: How to Build Better Software Faster_. Leanpub. Available at: [https://leanpub.com/cd-pipelines](https://leanpub.com/cd-pipelines) (Accessed: 22 November 2025).

[^30]: Continuous Delivery Ltd. (no date) 'Dave Farley on How to Refactor Bad Legacy Code'. _CD Training_. Available at: [https://courses.cd.training/courses/refactoring-tutorial](https://courses.cd.training/courses/refactoring-tutorial) (Accessed: 22 November 2025).

[^31]: Farley, D. (2022) 'What Software Architecture Should Look Like?'. _YouTube_, 30 March. Available at: [https://youtu.be/8GONv6jJsG0](https://youtu.be/8GONv6jJsG0) (Accessed: 22 November 2025).

[^32]: Farley, D. (2022) 'What Software Architecture Should Look Like?'. _YouTube_, 30 March. Available at: [https://youtu.be/ElMnHDSFaCw](https://youtu.be/ElMnHDSFaCw) (Accessed: 22 November 2025).

[^33]: Farley, D. (2025) 'The Pros & Cons of Pair Programming (With Examples)'. _YouTube_, 5 February. Available at: [https://youtu.be/fbxMV76e7_E](https://youtu.be/fbxMV76e7_E) (Accessed: 22 November 2025).

[^34]: Farley, D. (2022) 'Improving Observability and Testing in Production'. _YouTube_, 3 August. Available at: [https://youtu.be/Nmu4URA7pSM](https://youtu.be/Nmu4URA7pSM) (Accessed: 23 November 2025).

[^35]: Ukis, V. (2022) _Establishing SRE Foundations_. Available at: [https://amzn.to/3MbcT5C](https://amzn.to/3MbcT5C) (Accessed: 23 November 2025).

[^36]: Forsgren, N., Humble, J. and Kim, G. (2018) _Accelerate: The Science of Lean Software and DevOps – Building and Scaling High Performing Technology Organizations_. Portland, OR: IT Revolution.

---

## 本文書の用語 {#glossary}

本文書で使用される主な用語の解説です。Scrum Guide Expansion Packの他の文書で共通して使用される用語については、[用語集（スクラムガイド拡張パック 2026.1）]({{< ref "/scrum-guide-expanded/2026.1/index.ja.md#glossary" >}})を参照してください。

### ソフトウェアエンジニアリングプラクティス固有の用語

| 英語 | 日本語 | 説明 |
|------|--------|------|
| Continuous Integration (CI) | 継続的インテグレーション | チームメンバーが少なくとも毎日変更をマージし、自動ビルドで検証するプラクティス |
| Continuous Delivery (CD) | 継続的デリバリー | ソフトウェアを常にリリース可能な状態に保つプラクティス |
| Continuous Deployment | 継続的デプロイメント | 成功した変更を自動的に本番環境にプッシュするプラクティス |
| Test-Driven Development (TDD) | テスト駆動開発 | コードを書く前にテストを書く開発アプローチ |
| Deployment Pipeline | デプロイメントパイプライン | 変更がリリース可能かを判定するエンドツーエンドの自動化プロセス |
| Modularity | モジュール性 | システムのコンポーネントが分離・再結合できる度合い |
| Cohesion | 凝集度 | モジュール内の要素がどれだけ一緒に属しているかの度合い |
| Separation of Concerns | 関心の分離 | プログラムを別々のセクションに分離する設計原則 |
| Abstraction | 抽象化 | より重要な詳細に注意を集中させるために詳細を除去するプロセス |
| Coupling | 結合度 | ソフトウェアモジュール間の相互依存の度合い |
| Big Ball of Mud | 巨大な泥だんご | 構造がなく、誰もが変更を恐れるレガシーシステム |
| Feature Flag | フィーチャーフラグ | ユーザーがどのバージョンの機能と相互作用するかを選択できるスイッチ |
| Dark Launching | ダークローンチング | 部分的に完成した機能をユーザーに見えないように隠す技法 |
| Trunk-based Development | トランクベース開発 | 作業を統合された状態に保ち、マージコンフリクトを減らす開発手法 |
| Infrastructure as Code | Infrastructure as Code | インフラストラクチャの構成をコードとして管理する手法 |
| DORA Metrics | DORAメトリクス | 安定性とスループットを測定するソフトウェアデリバリーの指標 |
| Stability | 安定性 | エンジニアが構築するシステムの品質 |
| Throughput | スループット | エンジニアがその品質の変更を提供できる速度 |
| Observability | オブザーバビリティ | 実行中のシステムの状態を理解・監視する能力 |
| Telemetry | テレメトリ | 実行中のシステムからのデータ収集と監視 |

