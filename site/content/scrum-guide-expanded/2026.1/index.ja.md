---
# title: Scrum Guide Expanded
title: スクラムガイド拡張版
# description: The Scrum Guide Expansion Pack is a comprehensive companion to the 2020 Scrum Guide, created to help professionals navigate today's complex product environments. It deepens understanding of core Scrum principles by offering additional guidance on complexity, product thinking, systems of work, and leadership; while remaining true to Scrum's ethos of empiricism and self-management.
description: スクラムガイド拡張パックは、2020年版スクラムガイドの包括的な副読本として、現代の複雑なプロダクト環境を歩むプロフェッショナルの手助けとなるべく作成された。複雑性・プロダクト思考・仕事のシステム的捉え方・リーダーシップについて、追加のガイダンスを提供することで、スクラムの核となる原則の理解を深める。同時に、経験主義と自己管理というスクラムの精神に忠実であり続ける。
# keywords:
#   - Scrum
#   - modern Scrum
#   - Product Management
#   - empirical product development
#   - Scrum in complex environments
#   - Scrum and AI
keywords:
  - スクラム
  - モダンスクラム
  - プロダクトマネジメント
  - 経験的プロダクト開発
  - 複雑な環境でのスクラム
  - スクラムとAI
author:
  - Ralph Jocham
  - John Coleman
  - Jeff Sutherland
translators:
  - name: 内山遼子
    githubUsername: RyokoUchiyama
    url: https://www.linkedin.com/in/ryoko-uchiyama-0b870aa1/
    role: translator
    weight: 1
  - name: 川⼝恭伸
    githubUsername: kawaguti
    url: https://www.linkedin.com/in/yasunobu-yesno-kawaguchi-b78ab65/
    role: translator
    weight: 2
  - name: 長沢智治
    githubUsername: tomoharunagasawa
    url: https://nagasawa.social/
    role: translator
    weight: 3
  - name: 山本尊人
    githubUsername: Sonjin-Yamamoto
    url: https://www.linkedin.com/in/sonjin/
    role: translator
    weight: 4
  - name: 和⽥圭介
    githubUsername: k8skwada
    url: https://www.linkedin.com/in/wadak8sk/
    role: translator
    weight: 5
date: 2026-01-18T09:00:00Z
type: guide
lang: ja
mainfont: "Times New Roman"
sansfont: "Arial"
monofont: "Courier New"
forked_from: scrum-guide-expanded/2025.6
sitemap:
  priority: 0.8
aliases:
  - /ja/scrum-guide-expansion-pack/2026.1/
---

<!-- **_Collected Resources for Scrum Guide Expansion Pack_** -->

**_スクラムガイド拡張パック収録資料_**

<!-- _This document is a collection of independent works. Each section retains its original license or copyright status, as indicated. Please refer to each section for specific usage rights and requirements._ -->

_本書は、独立した著作物を収録したものである。各セクションは記載の通り、オリジナルのライセンスや著作権状況を保持している。特定の使用権限と要件については、各セクションを参照して欲しい。_

<!-- _Source: [2020 Scrum Guide](https://scrumguides.org/), [Scrum Guide Expansion Pack](https://scrumexpansion.org)_ -->

_出典：[2020年版スクラムガイド](https://scrumguides.org/)、[スクラムガイド拡張パック](https://scrumexpansion.org)_

<!-- _License: Creative Commons Attribution-ShareAlike 4.0 International ([CC BY-SA 4.0](https://creativecommons.org/licenses/by-sa/4.0/))._ -->

_ライセンス：クリエイティブ・コモンズ 表示-継承 4.0 国際（[CC BY-SA 4.0](https://creativecommons.org/licenses/by-sa/4.0/)）_

<!-- © _2025 Ralph Jocham, John Coleman, and Jeff Sutherland._ -->

© _2025 Ralph Jocham、John Coleman、Jeff Sutherland_

<!-- _Modification Notice: This is an adaptation of the original [2020 Scrum Guide](https://scrumguides.org/). Changes have been made from the original._ -->

_改変通知：これは[2020年版スクラムガイド](https://scrumguides.org/)を今日に適応させるものであり、オリジナルとは異なる内容を含みます。_

<!-- _Disclaimer: No warranties are given. Use at your own risk._ -->

_免責事項：いかなる保証も提供されない。各自の責任で利用して欲しい。_

<!-- _This section is offered under the Attribution-ShareAlike 4.0 International license of Creative Commons._ -->

_このセクションは、クリエイティブ・コモンズの表示-継承4.0国際ライセンスの下で提供されている。_

<!-- _By using this Scrum Guide Expansion Pack, you agree to the terms of the [CC BY-SA 4.0](https://creativecommons.org/licenses/by-sa/4.0/) license._ -->

_このスクラムガイド拡張パックを使用することで、[CC BY-SA 4.0](https://creativecommons.org/licenses/by-sa/4.0/)ライセンスの条項に同意したものとみなされる。_

---

<!-- ## Background -->

## 背景 {#background}

<!-- Jeff Sutherland's 1993 Scrum adoption at Easel was inspired by Christopher Langton's papers [1-2] on Complex Adaptive Systems (CAS) [3-6] theory from Los Alamos Labs, which showed that systems evolve quicker at the edge of chaos. -->

Jeff Sutherlandが1993年にEasel社でスクラムを採用したのは、ロスアラモス研究所のChristopher Langtonによる複雑適応系（CAS）[3-6]理論に関する論文[1-2]に触発されたものであった。この理論は、システムはカオスの縁でより速く進化することを示していた。

<!-- Ken Schwaber and Jeff Sutherland led the development of the Scrum framework. The [2020 Scrum Guide](https://scrumguides.org/) [7], including Ralph Jocham's contribution [8], describes the Scrum Essentials; Tobias Mayer's [A Simple Guide to Scrum](https://scrum.academy/guide/) [9] is a short version, and the [Scrum Hexis](https://thecynefin.co/product/hexi-scrumorg/?srsltid=AfmBOorcohLYeVy0qBsQFI6mK_bZtJA_uGC6hPL2BdptiTwNmMwpKTQv%20) [10] elaborate from a 2025 perspective. This document explains a lot about Scrum and offers guidance for the current times, but in the end, it departs in some places. Notable departures from the 2020 Scrum Guide are written like this (sometimes with an explanation). -->

Ken SchwaberとJeff Sutherlandがスクラムフレームワークの開発を主導した。[2020年版スクラムガイド](https://scrumguides.org/)[7]は、Ralph Jochamの貢献[8]を含め、スクラムの本質を説明している。Tobias Mayerの[A Simple Guide to Scrum](https://scrum.academy/guide/)[9]は短縮版であり、[スクラム ヘキシス](https://thecynefin.co/product/hexi-scrumorg/?srsltid=AfmBOorcohLYeVy0qBsQFI6mK_bZtJA_uGC6hPL2BdptiTwNmMwpKTQv%20)[10]は2025年の視点から詳述している。本書はスクラムについて多くを説明し、現代に向けたガイダンスを提供するが、最終的にはいくつかの点で異なる部分がある。2020年版スクラムガイドからの顕著な逸脱は、このように記述される（説明が付く場合もある）。

<!-- ## Purpose of the Scrum Guide Expansion Pack -->

## スクラムガイド拡張パックの目的 {#purpose-of-the-scrum-guide-expansion-pack}

<!-- This Scrum Guide Expansion Pack(SGEP) explains the _what_ and _why_ of each element of Scrum for the current times. Each element serves a specific purpose and contributes to the overall value and results realized with Scrum. This Expansion Pack will evolve regularly. The reader is expected to read the document sequentially, at least the first time. -->

このスクラムガイド拡張パック（SGEP）は、現代に向けてスクラムの各要素の _何_ と _なぜ_ を説明する。各要素は特定の目的を担い、スクラムで実現される全体的な価値と結果に貢献する。この拡張パックは継続的に進化していく予定だ。読者には前から順に読んでいくことを期待している。少なくとも一度目はそうしてほしい。

<!-- This document assumes some fluency with Scrum and its related language. It could be helpful to read the 2020 Scrum Guide first before reading this document. References are included for attribution purposes. Further, the related SGEP documents including references provide an opportunity for the reader to explore, research and learn to gain a broader and deeper understanding. -->

本書は、スクラムおよび関連用語について、ある程度理解している読者を想定している。この文書を読む前に、2020年版スクラムガイドを読んでおくと役立つだろう。出典明示のため、参考文献を記載している。さらに、参考文献を含む関連するSGEP文書は、読者がより広く深い理解を得るために探求し、研究し、学習する機会を提供する。

<!-- Practitioners and stakeholders should adopt Scrum when appropriate, with agency, urgency, courage, transparency, inspection, adaptation, rhythm, and resilience, and continually improve to support goals for the product (outcomes for users) and the organization (impact for the business). Scrum adoptions should surpass the guidance presented here and, in doing so, inspire a lasting curiosity to explore, question, and continually improve. -->

実践者とステークホルダーは、適切な場合にスクラムを採用すべきである。すなわち、主体性・緊急性・勇気・透明性・検査・適応・リズム・回復力を持って、プロダクト（ユーザーへのアウトカム）と組織（ビジネスへのインパクト）の目標を支援すべく継続的に改善する場合である。スクラムを適用することで、この文書で提示されたガイダンスを超越することを期待している。持続的な好奇心を持って、探求・問い・継続的な改善へと繋げてほしい。

<!-- This Expansion Pack is designed to support various aspects of product delivery by a self-managing team [11] driven by stakeholder needs or wants in response to a problem or opportunity. This includes (but is not limited to) product discovery, development, delivery, and value realization. While originally rooted in software product development, Scrum has been widely adopted across various domains, enabling the delivery of value through complex [12-17] work. As its use expands, professionals such as engineers, programmers, researchers, analysts, lawyers, marketers, and scientists increasingly apply Scrum successfully to their fields. -->

この拡張パックは、自己管理チーム[11]によるプロダクトデリバリーの様々な側面を支援するよう設計されている。そうしたチームは、問題や機会に対するステークホルダーのニーズや要望を原動力としている。これにはプロダクト発見・開発・デリバリー・価値実現が含まれる（ただしこれらに限定されない）。もともとソフトウェアプロダクト開発から始まったスクラムは、現在は多様な領域で幅広く採用され、複雑な[12-17]仕事を通じた価値の提供を可能にしている。利用が拡大するにつれ、エンジニア・プログラマー・研究者・アナリスト・弁護士・マーケター・科学者などの専門家が、それぞれの分野でスクラムを効果的に適用する例が増えている。

<!-- Stakeholder value (SG2020 only talks about value generically) refers to any perceived need that a stakeholder (including but not limited to customers, decision-makers, and users) considers important and that a team delivers. However, stakeholders may not always be aware of what could be valuable to them. Observation or evidence could intentionally or unintentionally surface value and influence priorities. As new information arises, potentially valuable items should be identified, inspected, refined, and adapted. Value remains an assumption until confirmed by evidence, such as observation or measured outcomes (and when aggregated, their impact on the organization). -->

ステークホルダー価値（SG2020では価値について一般的にしか述べていない）とは、ステークホルダーが重要と考え、チームが提供する、あらゆるニーズである（ステークホルダーには顧客、意思決定者、ユーザーを含むがこれらに限定されない）。ただしステークホルダー自身が、自分たちにとって価値あるものが何であるかを、かならずしも認識しているわけではない。観察やエビデンスを通じて、意図的もしくは意図しないところで価値が顕在化し、それが優先順位に影響を与えることがある。新しい情報が出てきたら、潜在的に価値のあるアイテムを特定し、検査し、リファインし、適応させるべきである。価値とは、観察や計測されたアウトカム（および集約された場合、組織へのインパクト）などのエビデンスによって確認されるまでは、あくまで仮説にすぎない。

<!-- ## Scrum in a Nutshell -->

## スクラム早わかり {#scrum-in-a-nutshell}

<!-- Scrum is a framework for complex [12-17] Product delivery, where expertise is valuable but more than expertise is needed, and cause and effect are only coherent in retrospect. Scrum addresses the full Product lifecycle, which includes (but is not limited to) creating, replacing, sustaining, adapting, continuously changing, maintaining, and retiring Products or features. Scrum helps individuals, teams, and organizations become and stay flexible and create value by adapting to change. -->

スクラムは、複雑な[12-17]プロダクトデリバリーのためのフレームワークである。専門性の価値を認めつつも、専門性を超えたものが必要であり、原因と結果の関係は、後から振り返ってこそ見えてくるものである。スクラムは、プロダクトライフサイクル全体をカバーする。そこには、プロダクトや機能の作成・置換・維持・適応・継続的変更・保守・廃止が含まれる（ただしこれらに限定されない）。スクラムは、個人・チーム・組織が変化に適応し、柔軟性を保ちながら価値を創造するのを支援する。

<!-- Scrum fosters a setting for understanding and coherently responding to Stakeholder needs. Scrum's iterative and incremental approach reduces risk and fosters continuous improvement. Scrum helps a team to strike a balance between exploring problems, discovering Stakeholder (including but not limited to customer) needs, delivering solutions, proactively managing risk, and validating value (user outcomes) and observing impact (business results). -->

スクラムはステークホルダーのニーズを理解し、一貫して対応するための環境を育む。スクラムのイテレーティブ（反復的）でインクリメンタル（漸進的）なアプローチはリスクを削減し、継続的改善を促進する。スクラムはチームが問題の探求、ステークホルダー（顧客を含むがこれに限定されない）のニーズの発見、ソリューションの提供、積極的なリスク管理、価値（ユーザーアウトカム）の検証とインパクト（ビジネス成果）の観察のバランスを取ることを支援する。

<!-- A risk is any factor that could result in a future adverse consequence. Since risk exposure remains unpredictable even as time elapses, anticipation is key. Risk exposure can include (but is not limited to) market risk, problem-solution fit, Product-market fit, technology, signal detection, responsiveness, compliance, remediation, poor trade-off decisions, etc. Scrum supports proactive risk management and opportunity discovery. -->

リスクとは、今後不利な結果をもたらしうる何らかの要因のことである。時間が経過してもリスクエクスポージャー（リスクの影響度）は予測不可能であり、あらゆる状況を見越した備え（anticipation）が鍵になる。リスクエクスポージャーには、次のものが含まれる（ただしこれらに限定されない）。市場リスク、プロブレム-ソリューションフィット、プロダクト-マーケットフィット、技術、シグナル検出、応答性、コンプライアンス、修復・再発防止、不適切なトレードオフ判断など。スクラムは積極的なリスク管理と機会発見を支援する。

<!-- Scrum encourages a reduction in the existing separation between Stakeholders who present problems or opportunities and the people solving them. -->

スクラムは、問題や機会を提示するステークホルダーとそれらを解決する人々の間にある距離を縮めることを奨励する。

<!-- In a nutshell, Scrum is based on an environment where: -->

一言で言うと、スクラムは以下のような環境に基づいている：

<!-- 1. Supporting Stakeholders, hereafter referred to as Supporters, doing what is requested to proactively support and enhance the adoption of Scrum, guided and supported by the Scrum Master. (SG2020 mentions stakeholder 14 times, never defines it) -->
<!-- 2. A Product Owner sets the Product Goal, instrumental in fulfilling Stakeholder value. -->
<!-- 3. The self-managing Scrum Team [11] defines, refines, and turns the selection of work into valuable outcomes. -->
<!-- 4. The Scrum Team and Stakeholders inspect the results during the Sprint and adapt. -->
<!-- 5. Supporters help the Scrum Team to thrive (SG2020 Supporter is not a concept). -->
<!-- 6. _Repeat._ -->

1. サポートステークホルダー（以下、サポーター）は、スクラムマスターの指導と支援のもと、要求されたことを実行し、スクラムの採用を積極的に支援し、促進する。（SG2020ではステークホルダーについて14回言及しているが、定義はされていない）
2. プロダクトオーナーがプロダクトゴールを設定し、ステークホルダー価値の実現に貢献する。
3. 自己管理スクラムチーム[11]が、選択された作業を定義し、リファインメントし、価値あるアウトカムに変える。
4. スクラムチームとステークホルダーがスプリント中に結果を検査し、適応する。
5. サポーターがスクラムチームの成功を支援する。（SG2020ではサポーターという概念はない）
6. _繰り返す。_

<!-- A release is the process of making a new or updated version of a Product available to Stakeholders (including but not limited to customers, decision-makers, and end users). It marks an inflection point in the development cycle and represents the transition of the Product from development to availability for use and the potential realization of Stakeholder value. -->

リリースとは、プロダクトの新バージョンまたは更新バージョンをステークホルダー（顧客、意思決定者、エンドユーザーを含むがこれらに限定されない）に提供するプロセスである。これは開発サイクルにおける変曲点であり、プロダクトが開発から利用可能な状態への移行と、ステークホルダー価値実現の可能性を表す。

<!-- Scrum is intentionally incomplete. Instead of prescribing detailed processes, it provides a framework that guides relationships and purposeful interactions. Various processes, techniques, and methods can complement Scrum, but their application depends on the context and varies across different uses of Scrum. -->

スクラムは意図的に不完全である。詳細なプロセスを規定する代わりに、関係性と意図的なインタラクションを導くフレームワークを提供する。様々なプロセス・技法・手法がスクラムを補完できるが、その適用は文脈に依存し、スクラムの使用方法によって異なる。

<!-- Scrum integrates with existing practices or, in some cases, makes them unnecessary or obsolete. By transparently assessing the effectiveness of the Scrum Team, Supporters, current management, work environment, and techniques, Scrum enables continuous improvement. -->

スクラムは既存のプラクティスと統合するか、場合によってはそれらを不要または時代遅れにする。スクラムチーム、サポーター、現在のマネジメント、作業環境、技法の有効性を透明性をもって評価することで、スクラムは継続的改善を可能にする。

<!-- In the context of knowledge work, the term Scrum, borrowed from the game of rugby, was coined by Hirotaka Takeuchi and Ikujiro Nonaka [18] to describe teams that worked this way and where knowledge was spread rapidly throughout an enterprise to deliver outstanding Products. -->

知識労働の文脈において、ラグビーから借用した「スクラム」という用語は、竹内弘高と野中郁次郎[18]によって作られた。これはこのような働き方をするチームを表し、優れたプロダクトを提供するために知識が企業全体に急速に広まることを示している。

<!-- ## Supporting and Complementary Theory -->

## 支援・補完理論 {#supporting-and-complementary-theory}

<!-- Scrum is founded on a self-managing Scrum Team [11], emergence, empiricism [19], and lean thinking [20]. It is underpinned by the supporting and complementary theory below and ideas such as: -->

スクラムは、自己管理スクラムチーム[11]、創発、経験主義[19]、リーン思考[20]を基盤としている。以下の支援・補完理論と、次のようなアイデアに支えられている：

<!-- - Accountability, -->
<!-- - The reduction of non-value-adding waste (including organizational inefficiencies), -->
<!-- - Framing work as problems or opportunities, -->
<!-- - Discovery, delivery, and value realization, and -->
<!-- - Continuous improvement. -->

- アカウンタビリティ（説明責任）
- 価値を生まないムダの削減（組織の非効率を含む）
- 仕事を問題または機会として捉えること
- 発見、デリバリー、価値実現
- 継続的改善

<!-- ## Complexity–The Case for Scrum -->

## 複雑性―スクラムの根拠 {#complexity-the-case-for-scrum}

<!-- For complex work, like building Products, there are more unknowns than knowns, expertise alone is valuable but insufficient, and cause and effect are only coherent in retrospect. Complexity thinking [12-17] provides valuable tools and ideas and facilitates insights. The Scrum Team members require time to think, help each other, do rework, or pivot. Cognitive diversity and empiricism can help deal with complex work. -->

プロダクト構築のような複雑な仕事では、既知のことよりも未知のことの方が多く、専門性だけでは価値があっても不十分であり、原因と結果は振り返ってみて初めて一貫性を持つ。複雑性思考[12-17]は価値あるツールとアイデアを提供し、洞察を促進する。スクラムチームのメンバーには、考える時間、互いに助け合う時間、やり直しやピボットの時間が必要である。認知的多様性と経験主義は、複雑な仕事に対処するのに役立つ。

<!-- Everything believed to be 'known,' including the market and Stakeholders (including but not limited to customers) can be wrong. Some expectations, needs, or wants emerge or fade away in relative importance or urgency over time. An empirical approach provides mechanisms for testing assumptions and inspecting and adapting. -->

市場やステークホルダー（顧客を含むがこれに限定されない）を含め、「既知」と信じられているすべてのことが間違っている可能性がある。期待・ニーズ・要望の中には、時間の経過とともに相対的な重要性や緊急性が現れたり消えたりするものがある。経験的アプローチは、仮説を検証し、検査・適応するためのメカニズムを提供する。

<!-- Generally, nothing stays in the same space forever. The Scrum Team might be on the edge of chaos, researching and working on something unprecedented, never done before. After a while, as they discover patterns and heuristics, it becomes less chaotic and more complex. After another while, for the situation at hand, the Scrum Team might move closer to the ordered space, something which is not easy but plannable. Or things can go in reverse. It is a good practice for the Scrum Team to pause and reflect if it's really in the space it thought it was in for the situation at hand. The key point is that Product development often deals with unpredictability, and Scrum can be a more useful approach than those with delusions of predictability. -->

一般的に、何事も永遠に同じ空間にとどまることはない。スクラムチームはカオスの縁にいて、前例のない、これまでにないことを研究し取り組んでいるかもしれない。しばらくすると、パターンやヒューリスティクスを発見するにつれ、カオス的ではなくなり、より複雑になる。さらにしばらくすると、その状況において、スクラムチームは秩序空間に近づくかもしれない。それは簡単ではないが計画可能なものである。あるいは、逆方向に進むこともある。スクラムチームが立ち止まって、その状況において本当に自分たちが考えていた空間にいるのかを振り返ることは、良いプラクティスである。重要な点は、プロダクト開発はしばしば予測不可能性を扱い、スクラムは予測可能性の幻想を持つアプローチよりも有用なアプローチになりうるということである。

<!-- The opportunities from emergence through Inspection and Adaptation of the _who_, _why_, _what_, _how_, _where_, and _when_ are plentiful. It's important to dampen what does not work and amplify what works. Transparency, Inspection, and Adaptation towards set goals, informed by result feedback (and unintended consequences), provide value creation, insights, risks, and challenged assumptions; this can foster continuous improvement. -->

_誰が_、_なぜ_、_何を_、_どのように_、_どこで_、_いつ_ の検査と適応を通じた創発からの機会は豊富にある。うまくいかないものを抑制し、うまくいくものを増幅することが重要である。結果のフィードバック（および意図しない結果）に基づいた、設定された目標に向けた透明性・検査・適応は、価値創造・洞察・リスク・仮説への挑戦を提供する。これにより継続的改善が促進される。

<!-- Build trust through a self-managing team, Inspection, Adaptation, delivering valuable work, and uncovering new insights. -->

自己管理チーム、検査、適応、価値ある仕事の提供、新しい洞察の発見を通じて信頼を構築する。

<!-- ## Emergence -->

## 創発 {#emergence}

<!-- Emergence [21] is when meaningful patterns or behaviors arise from interactions within complex [12-17] systems-patterns you can't predict just by looking at the parts alone. In Scrum, emergence isn't tightly controlled but is guided by enabling constraints like timeboxes, roles (re-introduced in SGEP), and feedback loops, which create the conditions for self-management and adaptability without dictating exact outcomes. These structures act like 'islands' in a sea of unpredictability, similar to how physical systems can spontaneously form organized patterns amid randomness, as described in Stephen Wolfram's work [22]. The key is that the structure in Scrum provides enough guidance for teams to self-manage and for new solutions to emerge rather than prescribing every detail. -->

創発[21]とは、複雑な[12-17]システム内のインタラクションから、意味のあるパターンや行動が生じることである。それは部分だけを見ても予測できないパターンである。スクラムにおいて、創発は厳密にコントロールされるのではなく、タイムボックス、ロール（SGEPで再導入）、フィードバックループのようなイネーブリング制約によって導かれる。これらは正確な結果を指示することなく、自己管理と適応性の条件を作り出す。Stephen Wolframの研究[22]で説明されているように、物理システムがランダム性の中で自発的に組織化されたパターンを形成できるのと同様に、これらの構造は予測不可能性の海の中の「島」として機能する。重要な点は、スクラムの構造がすべての詳細を規定するのではなく、チームが自己管理し、新しいソリューションが創発するのに十分なガイダンスを提供することである。

<!-- Scrum Teams, operating as complex adaptive systems, are influenced, not directed, through short, parallel, safe-to-fail experiments and continuous feedback. Patterns [23] like Swarming, Stable Teams, and Kaizen help identify and shape emergent behavior. Rather than forcing results, Scrum enables the Scrum Team to discover desirable patterns, including but not limited to innovative solutions or new ways of working, and amplify them while dampening unhelpful ones. -->

複雑適応系として機能するスクラムチームは、短期間で並行した、失敗しても安全な実験と継続的なフィードバックを通じて、指示されるのではなく影響を受ける。スウォーミング、安定したチーム、カイゼンなどのパターン[23]は、創発的な行動を特定し形作るのに役立つ。結果を強制するのではなく、スクラムはスクラムチームが望ましいパターン（革新的なソリューションや新しい働き方を含むがこれらに限定されない）を発見し、それらを増幅しながら役に立たないものを抑制することを可能にする。

<!-- This approach recognizes that self-management [11] is not something to be designed top-down but something to be discovered in the right environment—an environment that feels purposeful, coherent, and alive, echoing Christopher Alexander's 'Quality Without a Name' [24]. Ultimately, Scrum treats emergence not as a risk to be eliminated but as a force to be cultivated for excellence in Product development. -->

このアプローチは、自己管理[11]がトップダウンで設計されるものではなく、適切な環境で発見されるものであることを認識している。それは目的を持ち、一貫性があり、生き生きとした環境であり、Christopher Alexanderの「名前のない質」[24]に通じる。最終的に、スクラムは創発を排除すべきリスクとしてではなく、プロダクト開発における卓越性のために育成すべき力として扱う。

<!-- ## Self-Managing Scrum Team -->

## 自己管理スクラムチーム {#self-managing-scrum-team}

<!-- A self-managing [11] Scrum Team checks whether they are on track, takes action when not on track, decides how to work, resolves Scrum Team conflict, and fixes problems in the Scrum Team. This means that, generally, managers [25], if they are part of the landscape, do not tell the Scrum Team what to do or decide which Scrum Team member needs to be taken aside to fix issues, directly or indirectly. If managers exist it's generally better if they demonstrate leadership. -->

自己管理[11]スクラムチームは、自分たちが軌道に乗っているかを確認し、軌道に乗っていないときは行動を起こし、どのように働くかを決定し、スクラムチーム内の対立を解決し、スクラムチーム内の問題を修正する。これは一般的に、マネージャー[25]が存在する場合でも、スクラムチームに何をすべきかを指示したり、どのスクラムチームメンバーを呼び出して問題を修正すべきかを直接的または間接的に決定したりしないことを意味する。マネージャーが存在する場合、彼らがリーダーシップを発揮する方が一般的に良い。

<!-- Self-managing Scrum Teams organized around value are crucial for creative problem-solving and capturing emergence; reliance on non-self-managing Scrum Teams hinders the ability to deal with complexity [12-17]. Self-managing Scrum Teams [11] are not to be confused with individual self-management. It is the seamless interplay that allows a great team to emerge. The facilitation of team autonomy and more efficient decision-making within a non-hierarchical structure could help Scrum Teams improve their self-management. -->

価値を中心に組織された自己管理スクラムチームは、創造的な問題解決と創発の捕捉に不可欠である。自己管理でないスクラムチームへの依存は、複雑性[12-17]に対処する能力を妨げる。自己管理スクラムチーム[11]は、個人の自己管理と混同してはならない。偉大なチームが創発するのを可能にするのは、シームレスな相互作用である。非階層的な構造内でのチームの自律性の促進とより効率的な意思決定は、スクラムチームが自己管理を改善するのに役立つ可能性がある。

<!-- ## Professionalism -->

## プロフェッショナリズム {#professionalism}

<!-- Professionalism is about striving for excellence and working together to deliver value in a respectful, transparent, and accountable way. Being professional means that one will always do certain things and others never, regardless of the circumstances. -->

プロフェッショナリズムとは、卓越性を追求し、敬意を持ち、透明性があり、説明責任を果たす方法で価値を提供するために協力することである。プロフェッショナルであるとは、状況に関係なく、常に特定のことを行い、他のことは決して行わないことを意味する。

<!-- Being Professional means taking full accountability for the Product, from the cradle to the grave, throughout its entire life cycle. Being professional includes maintenance, often in the form of operations, and provides excellent engineering result feedback learning opportunities for the Product Developers. -->

プロフェッショナルであるとは、プロダクトのライフサイクル全体を通じて、ゆりかごから墓場まで、プロダクトに対する完全な説明責任を負うことを意味する。プロフェッショナルであることには、運用の形でのメンテナンスが含まれ、プロダクト開発者にとって優れたエンジニアリング結果フィードバックの学習機会を提供する。

<!-- In a software development context, professionalism includes but is not limited to technical excellence [26]. Technical excellence encompasses but is not limited to, the following: Specification by Example, Clean Code, Unit Testing, Test-Driven Development, Test Automation, Continuous Integration, Continuous Delivery, Architecture and Design, Acceptance Testing, and purposeful and intentional consideration of testing. -->

ソフトウェア開発の文脈では、プロフェッショナリズムには技術的卓越性[26]が含まれるがこれに限定されない。技術的卓越性には次のものが含まれるがこれらに限定されない：実例による仕様、クリーンコード、ユニットテスト、テスト駆動開発、テスト自動化、継続的インテグレーション、継続的デリバリー、アーキテクチャと設計、受け入れテスト、テストに対する意図的かつ計画的な考慮。

<!-- ## Lean Thinking -->

## リーン思考 {#lean-thinking}

<!-- 'Lean thinking [20] reduces waste in the work and how it is carried out, and focuses on the flow of value and continuous improvement.' The Lean principles are built on continuous improvement and respect for people. By focusing on the Lean principles, organizations can improve effectiveness at the lowest long-term costs and deliver better value to customers while fostering a climate of ongoing learning and development. -->

「リーン思考[20]は仕事とその遂行方法におけるムダを削減し、価値の流れと継続的改善に焦点を当てる。」リーンの原則は、継続的改善と人への敬意の上に構築されている。リーンの原則に焦点を当てることで、組織は最低の長期コストで効果性を向上させ、継続的な学習と成長の風土を育みながら、顧客により良い価値を提供できる。

<!-- ## Empiricism -->

## 経験主義 {#empiricism}

<!-- Empiricism [19] is the principle of making decisions informed by objective or observable evidence in learning cycles, often exploratory. It can be useful in situations where more than expertise is needed. Scrum is founded on empiricism. Decisions are informed by evidence or what is observed. An empirical approach involves ongoing observations, theory development/refinement, operationalization, and testing/modification to establish effective feedback loops. -->

経験主義[19]とは、学習サイクルにおいて、客観的または観察可能なエビデンスに基づいて意思決定を行う原則であり、しばしば探索的である。専門性だけでは不十分な状況で有用である。スクラムは経験主義を基盤としている。意思決定はエビデンスまたは観察されたものに基づいて行われる。経験的アプローチには、継続的な観察、理論の開発/洗練、運用化、効果的なフィードバックループを確立するためのテスト/修正が含まれる。

<!-- Empiricism can help Scrum Teams deliver something that Stakeholders find valuable when the _what_ or the _how_ is uncertain. Scrum is about making the improbable probable by discovering, delivering, and realizing value; this often includes but is not limited to trade-offs or experimentation. Experiments are generally based on testable hypotheses but sometimes on educated hunches. A key response to experimentation is evidence-informed decision-making. -->

経験主義は、_何を_ または _どのように_ が不確かなときに、ステークホルダーが価値があると感じるものをスクラムチームが提供するのに役立つ。スクラムとは、発見・デリバリー・価値実現を通じて、ありそうもないことを可能にすることである。これにはしばしばトレードオフや実験が含まれるがこれらに限定されない。実験は一般的にテスト可能な仮説に基づくが、時には経験に基づく直感に基づくこともある。実験への重要な対応は、エビデンスに基づいた意思決定である。

<!-- Pausing and reflecting combine elements of empiricism and lean thinking, create the basis for transparency, inspection, and adaptation toward the Product Goal, and help the Scrum Team and Supporters improve themselves and their environment. -->

立ち止まって振り返ることは、経験主義とリーン思考の要素を組み合わせ、プロダクトゴールに向けた透明性・検査・適応の基盤を作り、スクラムチームとサポーターが自分たち自身と環境を改善するのを助ける。

<!-- An effective Scrum adoption reduces the distance between Stakeholders who present problems or opportunities and the people dealing with them by keeping objectives tangible and meaningful and delivering value quickly and frequently. Stakeholders often have a mistaken sense of certainty about the what and the how. The Scrum Team often has a mistaken sense of certainty about who is impacted. Inspecting and adapting should be more valued than keeping promises or serving the wrong Stakeholders. All assumptions can be wrong. (SG2020 PO could be read as a proxy and value assumed) -->

効果的なスクラムの採用は、目標を具体的で意味のあるものに保ち、価値を迅速かつ頻繁に提供することで、問題や機会を提示するステークホルダーとそれらに対処する人々の間の距離を縮める。ステークホルダーは、何を、どのようにについて誤った確信を持っていることが多い。スクラムチームは、誰が影響を受けるかについて誤った確信を持っていることが多い。約束を守ることや間違ったステークホルダーに奉仕することよりも、検査と適応がより価値を持つべきである。すべての仮説は間違っている可能性がある。（SG2020のPOは代理人として読むことができ、価値は仮定されている）

<!-- ## Cadence -->

## ケイデンス {#cadence}

<!-- Working in Sprints provides a consistent rhythm that helps the Scrum Team focus on clear, short-term goals. This cadence supports regular inspection and adaptation, enabling the Scrum Team to learn and adjust informed by feedback. Over time, it builds a sustainable pace of delivery, improving predictability and fostering continuous improvement. -->

スプリントで働くことは、スクラムチームが明確で短期的な目標に集中するのを助ける一貫したリズムを提供する。このケイデンスは定期的な検査と適応をサポートし、スクラムチームがフィードバックに基づいて学習し調整することを可能にする。時間の経過とともに、持続可能なデリバリーのペースを構築し、予測可能性を向上させ、継続的改善を促進する。

<!-- ## The Three Pillars of Scrum's Empirical Process Control -->

## スクラムの経験的プロセス制御の三本柱 {#the-three-pillars-of-scrums-empirical-process-control}

<!-- Empiricism, at its core, is the philosophy that knowledge comes from experience and observation. Valuable insights emerge from curiosity, experience, experimentation, data, visualization, and observation. Empirical process control [27-29] is a method of managing complex [12-17] processes, like those in Scrum, by adapting informed by observed results, relying on the three pillars of transparency, inspection, and adaptation. -->

経験主義とは、その核心において、知識は経験と観察から得られるという哲学である。価値ある洞察は、好奇心、経験、実験、データ、可視化、観察から生まれる。経験的プロセス制御[27-29]は、透明性・検査・適応の三本柱に依拠し、観察された結果に基づいて適応することで、スクラムのような複雑な[12-17]プロセスを管理する方法である。

<!-- ## Transparency -->

## 透明性 {#transparency}

<!-- Transparency is a pillar of Scrum. It reveals reality and work clarity, and enables empiricism. Transparency reveals a more accurate perception of reality and is the entry point for Inspection and Adaptation. The emergent process, work, and results must be visible to those performing the work or receiving the inputs in the form of goals, Product Backlog Items, and associated outputs in the form of Increments. -->

透明性はスクラムの柱である。透明性は現実と仕事の明確さを明らかにし、経験主義を可能にする。透明性は現実のより正確な認識を明らかにし、検査と適応のエントリーポイントとなる。創発的なプロセス、仕事、結果は、仕事を行う人々、またはゴール・プロダクトバックログアイテムの形でインプットを受け取る人々、インクリメントの形で関連するアウトプットを受け取る人々に見えなければならない。

<!-- Important decisions are based on the artifacts, experiments, releases, or result feedback. Low Transparency can impair Inspection, leading to decisions that diminish value and increase risk. Transparency enables Inspection. -->

重要な意思決定は、アーティファクト、実験、リリース、または結果フィードバックに基づく。透明性が低いと検査が損なわれ、価値を減少させリスクを増加させる意思決定につながる。透明性は検査を可能にする。

<!-- Result feedback is data, ideally both quantitative and qualitative, that might result from changes to the Product or environment. It contributes to Stakeholder value, effort, resources, or costs. People are not resources. -->

結果フィードバックとは、プロダクトや環境への変更から生じる可能性のある、理想的には定量的かつ定性的なデータである。それはステークホルダー価値、労力、リソース、コストに寄与する。人はリソースではない。

<!-- Achieving Transparency is unrealistic and potentially inapplicable if there are institutional inefficiencies or there is a lack of trust. As a corollary, Scrum can make institutional inefficiencies transparent, and with collective will, trust can be built. -->

組織の非効率性がある場合や信頼が欠如している場合、透明性の達成は非現実的であり、適用できない可能性がある。当然の結果として、スクラムは組織の非効率性を透明にすることができ、集団的な意志があれば、信頼を構築できる。

<!-- ## Inspection -->

## 検査 {#inspection}

<!-- Inspection is a pillar of Scrum. Inspection is looking at reality, given the direction of the Product (the Product Goal) and the effectiveness of the Scrum Team and Stakeholders. Inspection enables Adaptation. Inspection is about looking at reality intentionally and is informed by the things that were made transparent, including evidence or observation. To foster Inspection and Adaptation, Scrum provides cadence in the form of its events. -->

検査はスクラムの柱である。検査とは、プロダクトの方向性（プロダクトゴール）とスクラムチームおよびステークホルダーの有効性を踏まえて、現実を見ることである。検査は適応を可能にする。検査とは、意図的に現実を見ることであり、エビデンスや観察を含む透明にされたものに基づいている。検査と適応を促進するために、スクラムはイベントの形でケイデンスを提供する。

<!-- The Scrum Artifacts, associated commitments, and progress toward agreed goals must be inspected frequently and diligently to detect emergence [21]. Inspection of the artifacts, experiments, releases, marketplace, or result feedback may yield learnings or side effects. Side effects are unexpected or unintended results or consequences. -->

スクラムアーティファクト、関連するコミットメント、合意された目標に向けた進捗は、創発[21]を検出するために頻繁かつ入念に検査されなければならない。アーティファクト、実験、リリース、市場、または結果フィードバックの検査は、学びや副作用をもたらす可能性がある。副作用とは、予期しない、または意図しない結果や帰結である。

<!-- Inspection without Transparency is ill-informed, misleading, and wasteful. -->

透明性のない検査は、情報不足であり、誤解を招き、無駄である。

<!-- ## Adaptation -->

## 適応 {#adaptation}

<!-- Adaptation is a pillar of Scrum. Given the direction of the Product, the Scrum Team and Stakeholders are expected to adapt to reality the moment improvement opportunities emerge, such as experiment outcomes, insights, risks, or opportunities. Adaptation becomes more difficult when institutional inefficiencies exist or when the people involved are not ready, willing, or able to do what needs to be done. -->

適応はスクラムの柱である。プロダクトの方向性を踏まえ、スクラムチームとステークホルダーは、実験結果・洞察・リスク・機会などの改善機会が現れた瞬間に、現実に適応することが期待される。組織の非効率性が存在する場合、または関係者が必要なことを行う準備・意欲・能力がない場合、適応はより困難になる。

<!-- Adaptation starts with accepting 'reality,' informed by evidence. Adaptation typically occurs in the Scrum Artifacts, associated commitments, Scrum Team, Stakeholders, leaders, and organization. If any aspects deviate outside acceptable limits or boundaries, or the resulting Product is unacceptable, adjustments must be made as soon as possible to course-correct. -->

適応は、エビデンスに基づいて「現実」を受け入れることから始まる。適応は通常、スクラムアーティファクト、関連するコミットメント、スクラムチーム、ステークホルダー、リーダー、組織において発生する。いずれかの側面が許容限度や境界を超えて逸脱した場合、または結果としてのプロダクトが受け入れられない場合は、軌道修正のためにできるだけ早く調整しなければならない。

<!-- Without Adaptation, Transparency and Inspection are meaningless. -->

適応がなければ、透明性と検査は無意味である。

<!-- ## The Scrum Values -->

## スクラムの価値基準 {#the-scrum-values}

<!-- The Scrum Values _—focus_, _openness_, _commitment_, _courage_, and *respect—*help create a Scrum Team environment that supports psychological safety and positive collaboration, which align with principles identified in neuroscience as beneficial for learning and effective teamwork. Consider the context. -->

スクラムの価値基準である、集中（_Focus_）、公開（_Openness_）、確約（_Commitment_）、勇気（_Courage_）、尊敬（_Respect_）は、心理的安全性と積極的なコラボレーションを促進するスクラムチームの環境をつくり、学習と効果的なチームワークに有益であると神経科学で特定された原則と整合している。文脈を考慮すること。

<!-- The Scrum Values foster transparency and trust, ensuring that words and actions align. Together, they create a strong foundation for collaboration, performance, and coherence within a Scrum Team. -->

スクラムの価値基準は透明性と信頼を育み、言葉と行動の一致を確保する。スクラムの価値基準を組み合わせることで、スクラムチーム内でのコラボレーション、パフォーマンス、一貫性のための強固な基盤が築かれる。

<!-- Successful Scrum adoption depends on the Scrum Team and Supporters (and other Stakeholders) leading by example as professionals. The Scrum Values can help improve trust among the Scrum Team and Stakeholders. The Scrum Values also encourage ethics [30], vocabulary, tone, work, behavior, and action that foster trust. They also help reduce or avoid a gap between words and actions. -->

スクラムの適用が成功するか否かは、スクラムチームとサポーター（およびその他のステークホルダー）がプロフェッショナルとして模範を示すことができるかどうかに依る。スクラムの価値基準は、スクラムチームとステークホルダー間の信頼を向上させるのに役立つ。スクラムの価値基準はまた、信頼を育む倫理[30]、語彙、トーン、作業、行動、アクションを促進する。それらはまた、言葉と行動の間のギャップを減らしたり避けたりすることを支援する。

<!-- The Scrum Team and Supporters agree to be _open_ about all the work and the challenges. Humility supports _Openness_. _Openness_ requires trust, and trust requires _Openness_. The Scrum Team and Supporters should request and share constructive feedback. They routinely collaborate and learn through high-bandwidth conversations and qualitative or quantitative feedback. -->

スクラムチームとサポーターは、すべての作業と課題について _公開_ であることに同意する。謙虚さは _公開_ を支える。_公開_ は信頼を必要とし、信頼は _公開_ を必要とする。スクラムチームとサポーターは建設的なフィードバックを要求し、共有すべきである。彼らは日常的に帯域幅の太い会話と定性的または定量的フィードバックを通じてコラボレーションし、学習する。

<!-- High-bandwidth conversations are conversations that foster communication in ways that allow for the richest, fastest, and clearest exchange of information. This typically involves face-to-face discussions-either in person, via video calls, visual management, or whiteboards (physical or digital), where participants can use not just words, but also tone of voice, facial expressions, drawing, or body language to fully understand each other. -->

帯域幅の太い会話とは、最も豊富で、最も速く、最も明確な情報交換を可能にする方法でコミュニケーションを促進する会話である。これは通常、対面での議論 —— 対面、ビデオ通話、視覚的管理、またはホワイトボード（物理的またはデジタル）を通じて —— を含み、参加者は言葉だけでなく、声のトーン、表情、描画、またはボディランゲージを使用して互いを完全に理解することができる。

<!-- As Sprints are short, any failures should be small and quick, and risk is identified and managed through fast and _open_ feedback. Perhaps, the only real failure is the lack of learning. -->

スプリントは短いため、小さく速く失敗すべきだ。リスクは迅速でオープン（_公開_）なフィードバックを通じて特定され、管理される。おそらく、真の失敗は唯一、学習の欠如だけである。

<!-- The Scrum Team and Supporters should have the _Courage_ to do the right thing and face tough challenges. They should be courageous in exploring the unknown, changing direction, requesting and sharing information, and engaging in courteous disagreements, e.g., healthy conflict and constructive dissent. The Scrum Team should ask Supporters and leaders for help if needed. -->

スクラムチームとサポーターは正しいことを行い、困難な課題に直面する _勇気_ を持つべきである。彼らは、未知の領域を探求し、方向転換を恐れず、情報の要求・共有を積極的に行い、真っ当な議論 —— 例えば、健全な対立や建設的な反対意見の表明など —— を交わす勇気を持つべきである。スクラムチームは必要に応じてサポーターとリーダーに助けを求めるべきである。

<!-- The Scrum Team _Commits_ to achieving the Sprint Goal, inspecting and adapting toward the Product Goal, (under-emphasized in SG2020) and supporting each other. Commitment means getting relevant work toward the Sprint Goal to comply with the Definition of Output Done at the latest by the end of the Sprint, preferably much earlier. Commitment also means getting to desired outcomes through value realization. -->

スクラムチームは、スプリントゴールの達成、プロダクトゴールに向けた検査と適応（SG2020では強調されていない）、そしてお互い助け合うことを _確約_ する。確約とは、スプリントゴールに向けた関連作業を、遅くともスプリント終了時までに、できればもっと早く、アウトプット完成の定義に準拠させることである。また確約とは、価値実現を通じて、望ましいアウトカムに近づいていくことでもある。

<!-- Their primary _Focus_ is making the best possible progress toward the Sprint Goal. Their secondary Focus is making the best possible progress toward the Product Goal. The Supporters _Commit_ to providing a psychologically safe space and environment for the Scrum Team to deliver Increments; within their _Focus_, the Scrum Team and Supporters _Commit_ to creating time for continuous learning and Adaptation, and the transfer of learning between Scrum Teams to ensure long-term effectiveness. The Scrum Team and Stakeholders should be intentional about addressing trade-offs, including consideration of short-term wins with long-term consequences. -->

スクラムチームが第一に _集中_ すべきことは、スプリントゴールに向けて可能な限り最善の進捗を遂げることである。スクラムチームが第二に _集中_ すべきことは、プロダクトゴールに向けて可能な限り最善の進捗を遂げることである。スクラムチームがインクリメントを届けるために、サポーターは心理的安全性の高い空間と環境を提供することを _確約_ する。その _集中_ を通じて、スクラムチーム・サポーターは継続的学習・適応およびスクラムチーム間での学習の移転の時間を作ることを _確約_ する。これらは長期的な効果性を確実にするためである。スクラムチームとステークホルダーは、短期的成果と長期的影響を考慮するなどのトレードオフに意図的に取り組むべきである。

<!-- The Scrum Team and Supporters (and other Stakeholders) _Respect_ each other as skilled professionals; they _Respect_ each other's differing expertise and perspectives and are constructive when disagreeing. Respectful behavior supports trust. The Scrum Team and Supporters should critique the idea or the approach to find more effective options, not the person(s). -->

スクラムチームとサポーター（および他のステークホルダー）は、熟練したプロフェッショナルとして互いを _尊敬_ する。お互いの異なる専門知識と視点を _尊敬_ し、意見の相違に対して建設的に対応する。尊敬ある行動は信頼を支える。スクラムチームとサポーターは、より効果的な選択肢を見つけるためにアイデアやアプローチを批評すべきであり、人を批判すべきではない。

<!-- _Respect_ helps protect against the weaponization of the other Scrum Values. Demonstrations of _Respect_ can include (but are not limited to) genuine praise, support for each other, humility, psychological safety, constructive disagreement, and cognitive diversity. -->

_尊敬_ は他のスクラムの価値基準が攻撃的に利用されることを防ぐ役割を果たす。_尊敬_ の実践には、心からの称賛、互いへの支援、謙虚さ、心理的安全性、建設的な意見の相違、認知的多様性などが含まれるがこれらに限定されない。

<!-- Scrum Team members and Stakeholders can look at the Scrum Values through the lens of John Boyd's OODA [99, 100, 102]. OODA was created by U.S. Air Force Colonel John Boyd to help pilots make quick, smart decisions in fast-changing situations by moving through four steps: Observe, Orient, Decide, and Act. It's a simple, continuous, iterative, powerful, if often subconscious way to handle uncertainty—like noticing market changes (Observe), analyzing trends and risks (Orient), choosing Product features to test (Decide), and delivering them (Act). OODA helps individuals stay flexible and respond well to whatever comes their way. Scrum can improve OODA. -->

スクラムチームメンバーとステークホルダーは、John BoydのOODA[99,100,102]の視点を通してスクラムの価値基準を見ることができる。OODAは、4つのステップ：観察（Observe）、状況判断（Orient）、意思決定（Decide）、行動（Act）を踏むことで、パイロットが急速に変化する状況で迅速かつ賢明な判断を行うことを支援するためにアメリカ空軍大佐John Boydによって作成された。OODAは不確実性を扱うためのシンプルで、継続的で、反復的で、強力な方法であり、しばしば無意識に活用される。例えば、市場変化に気づく（観察）、トレンドとリスクを分析する（状況判断）、テストするプロダクトフィーチャーを選択する（意思決定）、それらを提供する（行動）などである。OODAは個人が柔軟性を維持し、どんな状況にも適切に対応するのに役立つ。スクラムはOODAを改善できる。

<!-- Individual Scrum Team members can look at the Scrum Values through the lens of John Boyd's OODA, using Scrum to foster emergent solutions. In a Scrum context, the Scrum Values apply across all of OODA, (SGEP has a different emphasis) and in particular, help as follows: -->

スクラムチームメンバーはJohn BoydのOODAの視点からスクラムの価値基準を理解し、スクラムを活用して創発的なソリューションを育むことができる。スクラムの文脈では、スクラムの価値基準はOODAのすべてに適用され（SGEPでは強調点が異なる）、特に以下のように支援する：

<!-- - Observe—Openness and Respect can foster the gathering of all relevant evidence, and diverse perspectives.
- Orient—Courage is needed to interpret reality, navigate uncertainty, and agree to adapt or pivot, potentially using a reflective pause to challenge assumptions and provoke new insights.
- Decide—Deciding what to do requires timely analysis, such as backlog refinement, bringing potential next steps into Focus through parallel safe-to-fail experiments to test hypotheses, like small-scale probes (probes should be small, parallel, and designed so that failure is survivable and informative).
- Act—With clarity on what needs to be done, why, and by whom, Commitment can drive the team to execute effectively within enabling constraints like Sprint of determinant length, fostering emergent solutions. -->

- 観察：公開と尊敬は、関連するすべてのエビデンスと多様な視点の収集を促進する。
- 状況判断：現実を解釈し、不確実性を乗り越え、適応または方向転換に合意するには勇気が必要である。仮説を検証し新しい洞察を導き出すために、立ち止まって振り返ることもある。
- 意思決定：何をするかを決めるには、タイムリーな分析が求められる。バックログリファインメントなどを通じて、仮説を検証するための安全に失敗できる実験を並行して行い、次のステップに集中できるようにする（これらの実験は小さく、並行して実行ができ、失敗しても致命的でなく、かつ有益な情報をもたらすよう設計するべきである）。
- 行動：何を・なぜ・誰が行うかが明確であれば、確約によりスプリントの長さのような制約条件のもとでチームが効果的に行動し、創発的なソリューションを育むことができる。

<!-- ## More Supporting and Complementary Theory -->

## さらなる支援・補完理論 {#more-supporting-and-complementary-theory}

<!-- ## Product Thinking -->

## プロダクト思考 {#product-thinking}

<!-- People consume Products (including services), not projects. A Product is the conduit to deliver value, balancing the short- and long-term. This is why Scrum has a Product Owner and not a Project Owner. Products are long-term and need to be taken care of for their entire existence, whereas a project is timeboxed and often leaves an orphaned Product behind once the project is completed. -->

人々が実際に使うのはプロジェクトではなく、プロダクト（サービスを含む）である。プロダクトは、ユーザーに価値を届けるためのものであり、短期的な成果と長期的な視点の両方が求められる。そのため、スクラムでは「プロジェクトオーナー」ではなく「プロダクトオーナー」の役割が設けられている。プロダクトは長期間にわたって継続的に管理・改善していく必要があるが、プロジェクトはタイムボックスが決まっており、プロジェクトが完了するとプロダクトが十分にサポートされず放置されてしまうことがよくある。

<!-- Product thinking [31-33] deals with the tension [25] that Products often need to _Focus_ on growth in the short-term but also need to address long-term concerns, e.g., gaining traction with early adopters, 'crossing the chasm' [34], expanding, updating Product versions, continuous change, customer lifetime value and total cost of ownership. -->

プロダクト思考[31-33]とは、プロダクトが短期的な成長に _集中_ する必要がある一方で、長期的な課題にも対応しなければならないという葛藤[25]を扱う考え方である。たとえば、短期的には、アーリーアダプターを獲得し勢いを得ながら、プロダクトの利用を広げることが重要である。一方で、長期的には「キャズム（普及の壁）を超え」[34]、プロダクトを拡張し、バージョンアップや継続的な改善を行いながら、顧客のライフタイムバリュー（生涯価値）や総所有コストといった観点にも目を向ける必要がある。

<!-- To 'cross the chasm,' a strategy shift is needed from targeting savvy, risk-taking customers to winning over more pragmatic, risk-averse buyers, decision-makers, users, or other Stakeholders by focusing on a specific market area or target and delivering a complete, reliable solution that solves real problems. This step is crucial for a Product's transition from niche success to widespread adoption, as it moves from appealing to early adopters to attracting the early majority. The early majority often requires clear evidence of the Product's reliability and problem-solving capabilities within a specific context. By focusing on a niche and providing a complete solution, a company can build credibility, create reference customers, and establish a strong market position, effectively bridging the 'chasm' between early adopters and the mainstream market. -->

「キャズムを超える」には、新しいもの好きでリスクをいとわない顧客をターゲットにする戦略から、より現実的でリスク回避傾向が強い購入者や意思決定者、ユーザー、または他のステークホルダーを獲得するための戦略へとシフトする必要がある。そのためには、特定の市場やターゲット層に焦点を当て、実際の課題を解決できる、信頼性の高い完成度のあるソリューションを提供することが重要である。このステップは、一部のアーリーアダプターから、アーリーマジョリティに広く使われるようになるための分岐点となる。アーリーマジョリティは、特定の状況や用途でそのプロダクトが本当に信頼でき、問題解決に役立つという明確なエビデンスを求める傾向がある。ニッチな市場に集中し、完成度の高いソリューションを提供することで、企業は信頼を築き、他の顧客に紹介できる実績ある顧客（リファレンス顧客）を作り、市場での強固なポジションを確立できる。こうすることで、アーリーアダプターとメインストリームの市場の間にある「キャズム」を効果的に乗り越えることができる。

<!-- Product Owners need to master the handling of trade-offs between the _here_ and _now_ and the anticipated future (the _there_ and _then_) [35] through courage, humility, consultation, collaboration, healthy conflict, etc. -->

プロダクトオーナーは、勇気や謙虚さを持ち、周囲と相談したり協力したり、ときには建設的な意見のぶつかり合いを通じて、ここ（_Here_）と今（_Now_）と、予想される未来（そこ（_There_）とその時（_Then_））[35]の間のトレードオフを上手く扱う力が求められる。

<!-- Suppose the people involved are purely short-term thinkers. In that case, they will likely experience long-term side effects such as technical debt, low Scrum Team morale, busyness, output focus, etc. For that reason, mitigating factors would need to be put in place to support the long-term. -->

もし関係者が短期的な視点でのみ行動してしまうと、技術的負債がたまったり、スクラムチームの士気が下がったり、常に忙しくなったり、アウトプットばかりを重視してしまうなど、長期的にさまざまな副作用を経験する可能性がある。そのため、長期的な視点を持つための工夫や対策をあらかじめ用意しておく必要がある。

<!-- Technical debt is the extra work that builds up – consciously or unconsciously – when you take shortcuts in implementation or design to deliver something faster. Over time, it slows you down, just like real debt—with interest—because it makes future changes harder and riskier. Professionals strive to minimize technical debt and sloppiness as much as possible. If they decide to incur debt, it should be transparent, and if possible, an emergent mitigation plan should be in place. -->

技術的負債とは、何かをより早く提供するために、実装や設計で近道をした際に（意識的にしても無意識でも）積み重なっていく追加作業のことである。時間が経つにつれて、実際の借金のように（利子付きで）開発のスピードを落としてしまう。なぜなら、今後の変更を余計に難しく、リスクの高いものにするからである。プロフェッショナルならば、技術的負債・ずさんな作業をできるだけ最小限に抑えるよう努める。もし負債を負うことを決めたとしたら、それは透明性を持つべきであり、可能な限り、後から柔軟に対応できるような緩和策を用意しておくべきである。

<!-- For Products, Scrum supports feasibility, usability, desirability, value, and viability within ethical [30] boundaries through: -->

プロダクトに対して、スクラムは倫理的[30]な枠組みの中で、実現可能性、使いやすさ、魅力、価値、そして実行可能性を、以下を通じて支援する：

<!-- - Product design
- Product management
- Intentional consideration of the cohesive interplay of Stakeholders, research, goals, discovery, design, delivery, and continuous value realization
- In the specific case of technology Products, through Product engineering. -->

- プロダクト設計
- プロダクトマネジメント
- ステークホルダー、研究、ゴール、ディスカバリー、設計、デリバリー、継続的な価値実現といった要素が密接に連携し合うことを意識的に考慮すること
- 技術系プロダクトの場合は、プロダクトエンジニアリングを通じて

<!-- Scrum favors a healthy balance of the short-term and the long-term. Goal orientation enables potential outcomes through an emphasis on value and risk reduction. The Sprint Goal _(here_ and _now)_ should be a step toward the Product Goal _(there_ and _then)_, which enables pathways to the long-term. The Product Goal often supports the Product strategy and Product Vision. -->

スクラムは、短期と長期の健全なバランスを大切にする。ゴール指向で進めることで、価値の創出やリスク低減に重点を置き、潜在的なアウトカムを実現しやすくする。スプリントゴール（ここ（_Here_）と今（_Now_））は、プロダクトゴール（そこ（_There_）とその時（_Then_））に向かうための一歩であり、これが長期的な成長への道筋となる。プロダクトゴールは、プロダクト戦略やプロダクトビジョンを支える役割も果たす。

<!-- ## Systems Thinking -->

## システム思考 {#systems-thinking}

<!-- Systems thinking [36] acknowledges the interconnectedness of elements within organizational and social contexts, recognizing that actions in one area ripple in ways that aren't always predictable or linear. Theory-informed experiments, feedback loops, and follow-up data analysis help surface valuable and actionable insights. Systems Thinking provides valuable tools and ideas and facilitates insights. -->

システム思考[36]は、組織や社会の文脈において様々な要素が相互に結びついていることに着目し、ある領域での行動が必ずしも予測可能ではなく、また線形ではない方法で波及していくことを重視する考え方である。理論に基づく実験、フィードバックループ、追跡的なデータ分析を通じて、価値ある実践的な知見が得られる。システム思考は有用なツールとアイデアを提供し、洞察を促進する。

<!-- For an organization to become adaptive [37], it is necessary to avoid local sub-optimizations such as reducing unit costs while increasing long-term costs, eroding quality goals only to lose customer trust, or improving a Scrum Team, workflow, or process that should not exist. For complex work [12-17], it's not always possible to link cause and effect, except in hindsight. It's helpful, nevertheless, to consider possible and actual upstream, cross-stream, and downstream effects of interventions. -->

適応力[37]のある組織になるためには、個々のコストを削減しながら長期コストを増加させる、品質目標を犠牲にして顧客信頼を失う、そもそも存在すべきでないスクラムチーム、ワークフロー、プロセスを改善するなどの局所的な部分最適化を避けることが必要である。複雑な作業[12-17]では、原因と結果を結びつけることは必ずしもできず、多くの場合、事後に初めて理解できるものである。それでもなお、アクションや施策がもたらす前工程や関連領域、後工程に対する実際的もしくは潜在的な影響を考慮することは有用である。

<!-- ## Discovery -->

## ディスカバリー {#discovery}

<!-- Discovery [38-39] often starts with understanding people's expectations, needs, and wants through observation, analysis, conversations, and synthesis toward a desired outcome. Once a Scrum Team has gathered insights, it frames the problem or opportunity and orders them by potential value. The Scrum Team crowdsources possible solutions without judging them too quickly. If the potential value is high but there is a lack of evidence that the value can be realized, the Scrum Team should do research, assumption testing, or build simple prototypes they can test with real customers, decision-makers, or users. Discovery is never over; consider regular interviews or observations of customers, decision-makers, or users. -->

ディスカバリー[38-39]は、多くの場合、観察・分析・対話・統合を通じて人々の期待やニーズ、要望を把握し、望ましい成果を明確にすることから始まる。スクラムチームが十分な洞察を得たら、問題や機会を整理し、それらに潜在的な価値の大きさで優先順位を付ける。チームは急いで結論を出すことはせず、可能性のあるソリューションについて広くアイデアを集める。もし潜在的な価値が高いにもかかわらず、その価値が本当に実現できるというエビデンスが足りない場合は、追加の調査や仮説検証をする、あるいは実際の顧客・意思決定者・ユーザーに試せるシンプルなプロトタイプをつくるべきである。ディスカバリーは終わりのない活動であり、顧客や意思決定者、ユーザーへの定期的なインタビューや観察を続けることが推奨される。

<!-- Discovery is about learning toward a desired outcome through prioritizing, doing, avoiding, or constantly improving ideas informed by user observation, feedback, or other learnings. Discovery emphasizes collaboration, creativity, and not being afraid to fail and try again. Discovery frames work as problems or opportunities and helps the Scrum Team to create, prioritize, and test solution options that balance what people desire, what's technically possible, and what makes business sense—all while having fun. -->

ディスカバリーとは、ユーザー観察やフィードバック、その他の学びをもとに、アイデアの優先順位付け、実行、不要なものの見送り、そして継続的な改善を通じて、望ましい成果に向かって学び続ける活動である。ディスカバリーは、チームのコラボレーションや創造性を大切にし、失敗を恐れずに何度でも挑戦する姿勢を重視する。また、ディスカバリーによって、チームは作業を問題や機会として捉え直し、人々が望むもの・技術的に実現可能なこと・ビジネスとして意味があることのバランスを取りながら、さまざまな解決策の選択肢を生み出し、優先順位をつけて試すことができるようになる。そして、こうした活動全般をチームは楽しみながら行う。

<!-- If discovery is needed, it should (insofar as it is possible) be included in a manner that is consistent with Scrum. For example, discovery work is made transparent in the Product Backlog and Sprint Backlog, Scrum Team members practice discovery and other skills, learnings are discussed during the Sprint and at the Scrum events, and at least one Increment is produced (and ideally released) every Sprint, regardless of how much discovery is done. There is a balance to be struck: discovery can help avoid building the wrong thing, but it can be overdone, and, in the end, the result feedback matters the most. -->

ディスカバリーが必要な場合は、可能な限りスクラムと整合した形で取り入れるべきである。たとえば、ディスカバリーの作業はプロダクトバックログやスプリントバックログで可視化され、スクラムチームのメンバーはディスカバリーやその他のスキルを実践し、学びはスプリント中やスクラムイベントで議論される。そして、どれだけディスカバリーを行ったかに関わらず、毎スプリントで少なくとも一つのインクリメントが必ず作り出され（理想的にはリリースされ）るべきである。バランスを取ることが重要であり、ディスカバリーは間違ったものを作ることを防ぐのに役立つが、やりすぎることもあり得る。最終的には、結果からのフィードバック（結果フィードバック）が最も重要である。

<!-- ## Leadership -->

## リーダーシップ {#leadership}

<!-- Leadership is the ability to influence, guide, and inspire a group of people to achieve a common goal while avoiding demotivation. It inspires thoughts, actions, and passion and fosters clear strategic directions. It embraces purposeful and intentional Go See, Listen, and Understand, collecting facts and observations to inform decisions, better known as Genchi Genbutsu [40]. -->

リーダーシップとは、共通のゴールを達成するために、人々の意欲を低下させずに良い影響を与え、導き、鼓舞する能力である。それは思考、行動、情熱を刺激して、明確な戦略的方向性を育む。それは目的意識と意図を持って、現場を見る、聞く、理解するということを実践し、事実と観察結果を収集して意思決定に反映させるプロセスであり、現地現物[40]として知られている。

<!-- Leadership is a dynamic social process involving responsibility, relationship building, and empowerment. Successful leadership results in co-creating a direction of travel, effective alignment of resources and people needed, and mutual _Commitment_ among group members. -->

リーダーシップは、責任・人間関係構築・エンパワーメントを含んだ、動的で社会的なプロセスである。効果的なリーダーシップにより、進むべき方向の共創・必要なリソースと人材の効果的な配置・グループメンバー間の相互の _確約_ が実現される。

<!-- Scrum strives for a particular leadership, that is, leadership for resilience, a set of qualities, not a management position. Thus, leadership needs to include but not be limited to cultivating the environment for self-managing Scrum Teams, clarity, trust, transparency, emergence [21] in a direction, fulfillment at work, embracing uncertainty [41] and failures, gathering evidence for better decisions, proactively managing risk, and removing organizational inefficiencies. -->

スクラムにおけるリーダーシップとはすなわち、レジリエンスを重視するリーダーシップであり、管理職の地位ではなく一連の資質を指す。したがって、リーダーシップには、自己管理型スクラムチームの育成、明確さ、信頼、透明性、方向性における創発[21]、仕事における充実感、不確実性[41]と失敗の受け入れ、より良い意思決定のためのエビデンスの収集、積極的なリスク管理、組織の非効率性の除去などが含まれるが、これらに限定されない。

<!-- Leadership happens from all angles, should be at all levels, and fosters reflection at the right times. Leadership should drive ruthlessly for value, yet be compassionate and ethical. Leadership requires persistent agency to change workflows, processes, systems, and the work environment; this includes (but is not limited to) HR, finance, and vendor management. A leader is someone who demonstrates leadership. -->

リーダーシップはあらゆる方向から生まれ、すべてのレベルで存在すべきものであり、適切なタイミングで自らを振り返る契機ともなる。真のリーダーシップとは、価値の実現に向けて徹底的に取り組む姿勢を持ちつつも、常に思いやりと倫理観を忘れないことが求められる。リーダーシップには、ワークフロー、プロセス、システム、そして職場環境をより良くするための持続的な主体性が求められる。その取り組みは、人事、財務、ベンダー管理も含まれる（ただしこれらに限定されない）。つまり、リーダーとは、こうした姿勢をもってリーダーシップを発揮する人のことを指す。

<!-- Product Owners and Scrum Masters balance leadership, authority, and subtle control by providing clear intent, fostering initiative, and reinforcing accountability. They guide rather than micromanage, ensuring the Scrum Team understands the vision and goals, has the autonomy to execute, and remains accountable for outcomes. When intervention is needed, they step in decisively while preserving the Scrum Team's ownership of their accountabilities. Product Developers demonstrate leadership with their self-managing team orientation, professionalism, and goal orientation; self-management comes with responsibilities. Supporters demonstrate leadership by supporting short- and long-term impediment removal, improving the coherence of management processes with Scrum, and supporting emergent change in a powerful direction when requested. -->

プロダクトオーナーとスクラムマスターは、明確な意図を示し、自主性を促進し、責任感を高めることで、リーダーシップ・権威・そして微妙なコントロールのバランスを取る。彼らはマイクロマネジメントに陥ることなく、スクラムチームがビジョンとゴールを理解し、それを自律的に実行しながらアウトカムに対する説明責任を持ち続けるよう導く。介入が必要な場合は、スクラムチームのオーナーシップを保持させた上で、断固とした対応をとる。プロダクト開発者は、自己管理チーム指向、専門性、そしてゴール指向を通じてリーダーシップを発揮する。自己管理には責任が伴う。サポーターは、短期と長期の障害物除去の支援、スクラムとの整合性を高める管理プロセスの改善、要求に応じて明確な方向性に基づいた創発的な変化を後押しすることで、リーダーシップを発揮する。

<!-- ## First Principles Thinking -->

## 第一原理思考 {#first-principles-thinking}

<!-- First principles thinking is a method of problem-solving that involves breaking down challenges into their most fundamental truths and discovering solutions from the ground up. Instead of relying on analogy or established conventions, this approach asks, _'What do we know for certain?'_ and reconstructs understanding and solutions from those basic elements. Examples could include but are not limited to: -->

第一原理思考は、課題をその最も基本的な真実に分解し、根本から解決策を導き出す問題解決方法である。類推や確立された慣例に依存する代わりに、このアプローチは「確実に知っていることは何か？」と問い、それらの基本要素から理解と解決策を再構築する。例には以下が含まれるがこれらに限定されない：

<!-- - Encouraging the Scrum Team to _Focus_ on the core drivers of effectiveness, adaptiveness [37], and timeliness \-such as autonomy, transparency, and adaptation- rather than blindly following processes or copying what others have done. -->

- スクラムチームが盲目的にプロセスに従ったり、他チームの前例を模倣するよりも、自律性、透明性、適応といった効果性、適応性[37]、適時性を高める中核的要因に _集中_ することを促進する。

<!-- - Questioning every assumption and reconstructing solutions based on facts and essential principles, which can enable breakthroughs. -->

- あらゆる前提に疑問を持ち、事実と基本原理に基づいて解決策を再構築することで、ブレークスルーを可能にする。

<!-- - Advocating original thinking, continuous improvement, and the _Courage_ to challenge the status quo-unlocking creativity and enabling transformative results. -->

- 独創的な思考、継続的改善、現状に挑戦する _勇気_ を奨励し、創造性を解放し、変革を実現可能とする。

<!-- ## People and Change -->

## 人と変化 {#people-and-change}

<!-- The level of difficulty in adopting Scrum should not be underestimated. Scrum offers some guiding principles through its elements. It offers an approach to go back to first principles. -->

スクラム適用の難しさを過小評価すべきではない。スクラムは各構成要素を通じていくつかの道しるべとなる原則（guiding principles）を提供する。第一原理に立ち返るためのアプローチを提供している。

<!-- Scrum is not about adopting tools, short term delivery that sacrifices long term value. Often, incorrectly, Scrum practitioners only focus on short term impediment removal. Scrum requires change agency that balances the short term with the long term. -->

スクラムは、ツールの導入や長期的な価値を犠牲にした短期的なデリバリーの追求を目的とするものではない。スクラム実践者は、短期的な障害物の除去だけに終始してしまうことがよくある。しかしスクラムに必要なのは、短期と長期のバランスを取る変革推進力である。

<!-- A work related problem in Scrum could be anything that blocks or slows down progress, often addressed by self-managment of the Product Onwer and Product Developers. An impediment is a type of problem in Scrum and is anything that blocks or slows down progress and cannot be solved by the Developers & Product Owner. -->

スクラムにおける仕事上の問題とは、進捗を阻害または遅延させるあらゆるものを指し、多くの場合、プロダクトオーナーやプロダクト開発者による自己管理によって対処されるものである。障害物とはスクラムにおける問題の一種であり、進捗を阻害または遅延させるものであり、開発者やプロダクトオーナーだけでは解決できないものを指す。

<!-- It is crucial to be intentional, unrelenting, and tenacious about people, change, and communications. The change often includes people development, designs, workflows, processes, systems, attitudes, behaviors, language, habits, and the work climate. Culture is an emerging result. -->

人・変化・コミュニケーションについて、意図的に、手を緩めず、粘り強く取り組むことが必要不可欠である。変化には様々な要素が含まれる。人材開発、設計、ワークフロー、プロセス、システム、態度、行動、言語、習慣、職場環境などである。文化とは、そうした変化の創発的な結果である。

<!-- An effective Scrum adoption uses an emergent approach, has effective change agents (including Supporters and other Leaders), and engages enthusiastic support from those affected by it or affecting it. Intentionality and daily progress with the adoption are crucial; the adoption work should not be the last thing that is worked on after everything else is finished. -->

効果的なスクラムの適用は、創発的なアプローチの活用や効果的なチェンジエージェント（サポーターや他のリーダーを含む）の存在、そして、スクラムの影響を受ける人や影響を与える人たちの熱心な協力を得ることが必要である。スクラムの導入においては、意図的な取り組みと日々の進捗が重要であり、他のすべての作業が終わった後に最後に取りかかるものとしてはならない。

<!-- Start with disciplined emergent change in a direction. Strive to make emergent change a normality; eventually it becomes part of the scheduled work. A Scrum adoption has a direction but not a predefined destination. The change is emergent and therefore not predictable; a north star lights the path but is not a fixed destination. Curiosity enables a pattern of sense, listen, learn, and adapt in a direction. It's important to foster relationships and understand perspectives, and to listen to what is not being said and what is not happening. Change is hard work, yet fulfilling. -->

方向性を持ち、規律ある創発的変化から始めよう。創発的な変化を当たり前にして、やがてそれは定常的な仕事の一部になる。スクラムの適用には方向性はあるが、事前に定められた目的地はない。変化とは創発的なものであり、それゆえ予測できない。北極星が道を照らすことはあっても、それ自体が決まった目的地ではない。好奇心は、方向性を持った上で、感じる・聴く・学ぶ・適応するというパターンを可能にする。関係性を育み、多様な視点を理解し、語られていないことや起こっていないことに耳を傾けることが重要である。変化は困難だが、やりがいのある作業である。

<!-- Scrum Practioners and Supporters try not to be victims and do not rely on others to change. They try to make continual marginal changes within their grasp and create continual positive momentum. Ideally they are change catalysts and they radiate realistic positivity and possibilities. -->

スクラムの実践者とサポーターは、受け身の姿勢に甘んじず、他者の変化に依存しないように努める。自らの手の届く範囲で継続的に小さな変化を積み重ねることで、持続的な前向きな機運を生み出そうとする。理想的には、彼らは変化の推進役となり、実現可能な前向きさを広める存在である。

<!-- ## The Scrum Roles in the Expansion Pack -->

## 拡張パックにおけるスクラムの役割 {#the-scrum-roles-in-the-expansion-pack}

<!-- An accountability is a list of expectations that one is accountable for, e.g., the Product Owner accountable for value, the Scrum Master for the Scrum Team's effectiveness, and Product Developers for creating the usable Increment. Not all roles have accountabilities, i.e. Stakeholder. -->

説明責任とは、それぞれが説明責任を負うことになる期待事項のリストである。例えば、プロダクトオーナーは価値に対して説明責任を持ち、スクラムマスターはスクラムチームの効果性に対して説明責任を持ち、プロダクト開発者は有用なインクリメントの作成に対して説明責任を持つ。すべての役割が説明責任を持つわけではなく、その一例がステークホルダーである。

<!-- The four Scrum roles are Product Owner, Product Developer, Scrum Master, and Stakeholder. They give, reward, and earn trust and enable coherent leadership. Only the three accountabilities, Product Owner, Product Developer, and Scrum Master, are in the Scrum Team. -->

スクラムの4つの役割とは、プロダクトオーナー・プロダクト開発者・スクラムマスター・ステークホルダーである。これらは信頼を与え、信頼に報い、信頼を獲得し、一貫したリーダーシップを可能にする。スクラムチームに含まれるのは、プロダクトオーナー・プロダクト開発者・スクラムマスターの3つの説明責任のみである。

<!-- A person can hold more than one Scrum role. By taking on more than one role, one must be careful not to overstep. The Scrum roles are designed to keep check and balances in place. -->

1人が複数のスクラムの役割を担うことができる。複数の役割を担う場合、越権行為をしないよう注意しなければならない。スクラムの役割は、チェック・アンド・バランスを保つよう設計されている。

<!-- A Scrum Team is a team that practices Scrum, addresses three Scrum _accountabilities,_ namely, Scrum Master, Product Owner, and Product Developers, deals with Stakeholder (including but not limited to customer or user) problems or opportunities, and delivers useful, usable, and potentially valuable Increments from the perspectives of the Scrum Team and Stakeholders toward the Product Goal. For complex [12-17] work, a Scrum Team should be small, cognitively diverse, and self-managing, where human Scrum Team members, often assisted by technology, care about each other's work and learn how to do each other's work. -->

スクラムチームは、スクラムを実践し、スクラムマスター、プロダクトオーナー、プロダクト開発者というスクラムの3つの _説明責任_ を担い、ステークホルダー（顧客やユーザーを含むがこれらに限定されない）の問題や機会に対応し、スクラムチームとステークホルダーの視点から、プロダクトゴールに向けて有用で利用可能かつ潜在的に価値のあるインクリメントをデリバリーするチームである。複雑な[12-17]作業においては、スクラムチームは小規模で認知的多様性を持ち、自己管理型であるべきであり、人間のスクラムチームメンバーは、技術的な支援を受けながら、お互いの作業を気にかけ、お互いの作業のやり方を学ぶ。

<!-- The Scrum Team should be cross-functional, which means it is multidisciplinary, including technical and business domain skills. There is no explicit hierarchy within the Scrum Team. The Scrum Team should have all the skills and support needed to: -->

スクラムチームは機能横断型であるべきで、これは技術とビジネスドメインのスキルを含む多分野にわたることを意味する。スクラムチーム内に明示的な階層は存在しない。スクラムチームは以下に必要なすべてのスキルとサポートを備えるべきである：

<!-- - Discover (including research and design) as needed,
- Deliver (including engineering when appropriate); and,
- Validate value realization (and additionally usability, desirability, and viability within ethical [57] boundaries). -->

- 必要に応じてディスカバーする（調査と設計を含む）
- デリバリーする（適切な場合はエンジニアリングを含む）；そして
- 価値実現（および使いやすさ・魅力・倫理的な[30]境界内での実現可能性）を検証する。

<!-- The Scrum Team, supported by the Supporters, collectively takes care of the problem or opportunity domain, Product discovery, delivery, verification and built-in quality, go-to-market, and value validation toward the Product Goal. The Scrum Team strives for net improvements; being self-managing [11], they decide _who_ does _what_, _how_, _when,_ and _where_. -->

スクラムチームは、サポーターの支援を受けながら、問題や機会の領域、プロダクトのディスカバリー、デリバリー、検証、作り込み品質、市場投入、そしてプロダクトゴールに向けた価値検証に共同で取り組む。このチームは実質的な改善を目指し、自己管理[11]をしているため、_誰が_、_何を_、_どのように_、_いつ_、_どこで_、行うのかを自ら決定する。

<!-- Value validation is the confirmation (or disconfirmation) within given boundaries that the expected outcome(s) has been achieved. -->

価値検証とは、与えられた範囲内で、期待される結果が達成されたかどうかを確認（または棄却）することである。

<!-- The Scrum Team delivers an Increment(s) every Sprint, continuously self-manages [11] to find and fix problems, synchronizes continuously, and releases frequently. The Scrum Team is small enough to remain nimble and large enough to complete significant work within a Sprint. Often, smaller Scrum Teams communicate better and are more productive. -->

スクラムチームは毎スプリントでインクリメントを提供し、問題を発見して修正するために継続的に自己管理し[11]、継続的に同期し、頻繁にリリースする。スクラムチームは、俊敏性を保つのに十分な小ささと、スプリント内で重要な作業を完了するのに十分な大きさを持つ。多くの場合、より小さなスクラムチームの方がよりよくコミュニケーションを取り、より生産的である。

<!-- Scrum is built on self-managing Scrum Teams [11] within a defined organizational or Product structure. Autonomy exists, but it is bounded by Scrum events, accountabilities, artifacts, commitments, pillars, values, and organizational needs. -->

スクラムは、定義された組織またはプロダクト構造内の自己管理スクラムチーム[11]に基づいて構築されている。自律性は存在するが、スクラムイベント・説明責任・作成物・コミットメント・三本柱・価値基準・組織のニーズによって境界が設けられている。

<!-- Scrum engages groups of people who collectively have or acquire all the skills and expertise to do the work and share such skills as needed. Intentional interactions, supported by leaders, are needed to help improve the chances of successful outcomes. -->

スクラムは、作業に必要なすべてのスキルと専門知識を集合的に保有または習得し、必要に応じてそれらのスキルを共有する人々のグループを関与させる。成功につながるアウトカムの可能性を高めるために、リーダーによって支援された意図的な相互作用が必要である。

<!-- The _Focus_ should remain on achieving the Product Goal in the most effective way, with the right amount of investment, while delivering valuable outcomes. -->

_集中_ は、価値あるアウトカムを提供しながら、適切な投資量で最も効果的な方法でプロダクトゴールを達成することに向けられるべきである。

<!-- Scrum fosters collaborative teamwork by encouraging continuous interaction and shared accountability rather than sequential, siloed work. This approach enables the Scrum Team and Stakeholders to embrace uncertainty [41], allowing for quicker adjustments informed by ongoing learning and feedback. The overlapping nature of discovery, development, and value validation ensures a more adaptive [37], value-driven approach to Product development. -->

スクラムは、逐次的でサイロ化された作業ではなく、継続的な相互作用と共有説明責任を奨励することで、協調的なチームワークを促進する。このアプローチにより、スクラムチームとステークホルダーは不確実性[41]を受け入れることができ、継続的な学習とフィードバックに基づくより迅速な調整が可能になる。発見、開発、価値検証の重複する性質は、より適応的[37]で価値駆動型のプロダクト開発アプローチを保証する。

<!-- Overlapping work fosters shared accountability among the Scrum Team, enhancing engagement and commitment. The Scrum Team directs attention to addressing challenges and opportunities, encourages proactive behavior, cultivates a diverse skill set, and increases awareness of market dynamics among all participants. -->

重複する作業は、スクラムチーム内における説明責任の共有を促進し、エンゲージメントとコミットメントを高める。スクラムチームは、課題や機会への対応に意識を向け、自発的な行動を促し、多様なスキルセットを育成し、すべての関係者に市場動向への意識を高める。

<!-- The Scrum Team addresses all Product-related activities, from Stakeholder collaboration to value validation, including verification, maintenance, operation, experimentation, research and development, and anything else that might be required. The Scrum Team instills quality. Supporters ensure the organization structures the climate and the work environment and empowers the Scrum Team to self-manage [11]. Working in Sprints at a sustainable pace improves _Focus_ and consistency. -->

スクラムチームは、ステークホルダーとの連携から価値検証に至るまで、検証、保守、運用、実験、研究開発、その他必要とされるあらゆるプロダクト関連の活動を行う。スクラムチームは品質を作り込む。サポーターは、組織が適切な環境と作業環境を整備し、スクラムチームが自己管理[11]できるように支援する。持続可能なペースでスプリントで作業することは、_集中_ と一貫性を向上させる。

<!-- The Scrum Team and Stakeholders don't know what they will learn. Some learning provides greater certainty, and some creates more uncertainty [41]. Some things could emerge, fade away, drop out, or become less of a priority. -->

スクラムチームとステークホルダーは、何を学ぶことになるかを事前には知り得ない。ある学びは確実性を高める一方で、ある学びはさらなる不確実性[41]を生み出すこともある。いくつかのことは出現し、消え去り、脱落したり、優先度が低下したりする可能性がある。

<!-- A Scrum Team has aligned autonomy. Aligned autonomy means the Scrum Team has the freedom to decide how to solve problems while staying focused on shared goals and outcomes, enabling both innovation and organizational coherence. Fostering a cognitively diverse Scrum Team is essential. Cross-pollination is more likely when the Scrum Team members collaborate, trust each other, and can self-reflect. -->

スクラムチームは、整合性の取れた自律性を有している。整合性の取れた自律性とは、スクラムチームが共通の目標とアウトカムに集中しながらも、課題の解決方法を自ら決定できる自由を持つ状態を指し、イノベーションと組織としての一貫性の両立を可能にするものである。認知的多様性を持つスクラムチームを育成することは不可欠である。スクラムチームのメンバーが互いに協働し、信頼し合い、自己を内省できるとき、他家受粉がより促進される。

<!-- For successful outcomes, the Scrum Team and Supporters should cultivate a willingness to unlearn outdated principles. Inspection and Adaptation require a climate that anticipates and tolerates mistakes. It is essential to _Focus_ criticism on ideas rather than individuals. All Scrum Team members 'play on the same field' with coherently overlapping work, and are all accountable for success. -->

成功につながるアウトカムのためには、スクラムチームおよびサポーターが時代遅れの原則を手放す姿勢、すなわちアンラーンする意欲を育むことが求められる。検査と適応を実現するには、間違いを予期し許容する風土が不可欠である。批判は個人ではなく、アイデアに対して向けることに _集中_ する必要がある。スクラムチームのすべてのメンバーは「同じフィールドでプレーする」存在であり、作業は一貫性をもって重なり合い、成功に対して全員が責任を負う。

<!-- ## Stakeholder -->

## ステークホルダー {#stakeholder}

<!-- Stakeholder is a role. A Stakeholder is an entity, individual, or group interested in, affected by, or impacting inputs, activities, and outcomes. Stakeholders have a direct or indirect interest inside or outside the organization, its Products, or services. -->

ステークホルダーは役割の一つである。ステークホルダーとは、インプット・活動・アウトカムに関心を持ち、そこから影響を受けたり影響を与える存在・個人・グループである。ステークホルダーは、組織・プロダクト・サービスの内外に直接的・間接的な利害関係を持つ。

<!-- Examples of Stakeholders include (but are not limited to) customers, decision-makers, users, vendors, influencers, managers, colleagues, leaders, legislators, financial sponsors, subject matter experts, and governance oversight. Inanimate, non-human Stakeholders such as the law or AI should not be ignored. Some Stakeholders have more impact or are more impacted than others, and each can favor different factors. Each Stakeholder has a different degree of power or influence. -->

ステークホルダーには、顧客、意思決定者、ユーザー、ベンダー、インフルエンサー、マネージャー、同僚、リーダー、立法者、資金提供者、特定分野のエキスパート、ガバナンス監督者が含まれるが、これらに限定されない。法律やAIなどの無機物で人間ではないステークホルダーも無視すべきではない。ステークホルダーは、他のステークホルダーよりも影響力が強かったり、影響を受けたりする場合があり、優先する要素がそれぞれ異なる。ステークホルダーごとに権力や影響力の程度が異なる。

<!-- A customer is any Stakeholder who receives value from the Product by purchasing and/or selecting it. Customers may include buyers (those who pay for or acquire the Product), decision-makers (those who approve or authorize its adoption), and end users (those who interact directly with the Product). Sometimes, the customer is not the same as the end-customer, e.g., in B2B2C [42] or B2B2B [43]. -->

顧客とは、プロダクトを購入や選択することにより価値を受け取るステークホルダーの一種である。顧客には、購入者（プロダクトを購入または取得する人）、意思決定者（プロダクトの採用を承認または決定する人）、エンドユーザー（プロダクトを直接利用し、相互作用する人）が含まれる。B2B2C[42]やB2B2B[43]などのように、顧客と最終顧客が異なることがある。

<!-- For a successful Scrum adoption, it's crucial to have regular intentional interactions between Stakeholders (including but not limited to customers and users) and the Scrum Team. -->

スクラムの適用を成功させるためには、ステークホルダー（顧客とユーザーを含むがこれらに限定されない）とスクラムチームとの間で相互作用を生むやり取りを意図的かつ定期的に持つことが重要である。

<!-- A user is a Stakeholder who directly interacts with the Product to achieve specific goals or solve problems. Users experience the Product firsthand, whether it is a service, platform, or experience, and their feedback and satisfaction are crucial for ongoing Product improvement. Users may or may not have a say in purchasing decisions, but their adoption and engagement are essential for the Product's continued success. Sometimes, the user is not the same as the end-user, e.g., in B2B2C or B2B2B. For a successful Scrum adoption, it's crucial to have regular intentional interactions between users (and possibly end-users) and the Scrum Team. -->

ユーザーとは、特定の目標を達成するまたは課題を解決するためにプロダクトと直接相互作用するステークホルダーの一種である。ユーザーはサービス、プラットフォーム、体験などのプロダクトを実際に利用する。そのフィードバックや満足度はプロダクトの継続的改善に不可欠である。ユーザーは購入決定に発言権を持つ場合もあれば持たない場合もあるが、ユーザーによるプロダクトの利用とエンゲージメントはプロダクトの成功にとって重要である。B2B2CやB2B2Bなどのように、ユーザーとエンドユーザーが異なる場合もある。スクラムの適用を成功させるためには、ユーザー（必要に応じてエンドユーザーも）とスクラムチームとの間で相互作用を生むやり取りを意図的かつ定期的に持つことが重要である。

<!-- A decision-maker (called a 'chooser' by Jeff Patton) [44] is a Stakeholder with the authority to approve, select, or authorize the adoption or purchase of the Product. The decision-maker is responsible for evaluating options and making the final call, often considering the needs of both users and the broader organization. Decision-makers may or may not use the Product themselves, but their choices directly impact which Products are adopted and how value is delivered to other Stakeholders. For a successful Scrum adoption, it's often better to proceed with imperfect information, and capture emerging result feedback. -->

意思決定者[44]は、プロダクトの採用や購入を承認、選択、または決定する権限を持つステークホルダーの一種である。Jeff Pattonは「チューザー（選択者）」と呼んでいる。意思決定者は選択肢を評価し、最終判断を下す責任を負い、多くの場合、ユーザーや組織全体のニーズを考慮する。意思決定者自身がプロダクトを使用する場合もしない場合もあるが、彼らの選択はどのプロダクトが採用され、他のステークホルダーにどのように価値が提供されるかに直接影響する。スクラムの適用を成功させるためには、不完全な情報でも行動し、創発的な結果からのフィードバック（結果フィードバック）を捉えていくことが効果的である。

<!-- Legislators (plus, for the purpose of this document, external or internal policy makers) establish rules, policies, and boundaries for a Product's operation. They define legal, regulatory, or organizational frameworks that shape the Product's value delivery to Stakeholders and professionalism standards. They ensure the Product aligns with external or internal mandates, guiding its evolution and sustainability. For a successful Scrum adoption, it's crucial not to exaggerate or underestimate legal requirements. -->

立法者（加えて、この文書の目的に向けた外部または内部のポリシー立案者）は、プロダクトの運用に関するルール、ポリシー、境界を策定する。立法者はステークホルダーへのプロダクトの価値提供やプロフェッショナリズムの基準を形成する法的、規制的、または組織内の枠組みを定義する。立法者はプロダクトが外部や内部の要件に沿って進化し持続可能であるように導く。スクラムの適用を成功させるためには、法的要件を過大評価も過小評価もせず、適切に対応することが重要である。

<!-- Financial sponsors provide funding and resources for Product development, launch, and improvement. They assess the Product's viability, value, and feasibility, investing informed by its potential to deliver continuous value to Stakeholders. Financial sponsors influence the Product vision, strategy, and goals to ensure alignment with return on investment and long-term sustainability. For a successful Scrum adoption, it's crucial to have a flexible attitude and flexible funding as new information comes to light. -->

資金提供者は、プロダクト開発、リリース、改善のために資金やリソースを提供する。資金提供者はプロダクトの実現可能性、価値、実行可能性を評価し、ステークホルダーに継続的に価値を提供できる可能性を見極めて投資を行う。資金提供者は投資回収や長期的な持続性との整合を確かなものとするため、プロダクトのビジョン、戦略、目標に影響を与える。スクラムの適用を成功させるためには、新しい情報が明らかになるにつれて、柔軟に姿勢や資金運用を変えることが求められる。

<!-- Subject matter experts contribute deep knowledge or unique skills essential to Product creation, evolution, and maintenance. Whether focused on technology, design, compliance, or a specific domain, subject matter experts support the Product's usability, feasibility, professionalism, and extendability but do not get in the way of self-managing Scrum Teams [11]. They can help address satisfaction gaps and contribute to the Product's ability to adapt and identify, represent, or measure emergence [21]. For a successful Scrum adoption, it's crucial to foster regular transfer of learning from subject matter experts to and across the Scrum Team. -->

特定分野のエキスパートは、プロダクトの作成、進化、保守に不可欠な深い知識や独自のスキルを提供する。技術、設計、コンプライアンス、特定ドメインなどの分野で、特定分野のエキスパートはプロダクトの使いやすさ、実現可能性、プロフェッショナリズム、拡張性を支援するが、自己管理スクラムチーム[11]を妨げてはならない。特定分野のエキスパートは満足度ギャップを解消し、プロダクトが適応しやすくなるよう支援し、創発[21]を特定、表現、評価する役割を担う。スクラムの適用を成功させるために、特定分野のエキスパートからスクラムチームへ、そしてスクラムチーム全体への定期的な学びの移転を促進することが重要である。

<!-- The term satisfaction gap means the difference between what Stakeholders experience now and what they wish their experience was. In other words, it's the gap between how satisfied Stakeholders are with a Product today and how satisfied they could be. -->

満足度ギャップとは、ステークホルダーが現在体験していることと彼らが体験したいと望むこととの差を指す。言い換えれば、ステークホルダーが現在のプロダクトにどれだけ満足しているかと、ここからどれだけ満足させられるかとの間のギャップである。

<!-- Governance refers to structures, standards, regulations, norms, processes, and practices that consciously constrain and guide a Product's direction, decision-making, and accountability. Governance fosters transparency and guides adherence to standards of value, viability, and professionalism. It provides mechanisms for managing risks and adapting the Product to changing needs or environments, supporting its long-lived and evolutionary nature. For a successful Scrum adoption, it's crucial that governance is coherent with Scrum, e.g., a single point of contact per governance area, who has intentional interactions around quality and compliance with the Scrum Team, regular Inspection and Adaptation of the governance, and no surprises. -->

ガバナンスとは、プロダクトの方向性、意思決定、説明責任を意図的に制約する構造、標準、規制、規範、プロセス、プラクティスを指す。ガバナンスは透明性を促進し、価値、実現可能性、プロフェッショナリズムの基準への遵守を促進させる。ガバナンスはリスク管理を支援し、変化するニーズや環境に合わせてプロダクトを適応させるメカニズムを提供し、プロダクトを長期的に成長させ続ける土台を提供する。スクラムの適用を成功させるために、ガバナンスがスクラムと一貫性を持つことが重要である。たとえば、ガバナンス領域ごとに単一の連絡窓口を設定し、品質やコンプライアンスに関する意図的な対話をスクラムチームと行い、ガバナンス自体を定期的に検査・適応し、予期せぬ事象が生じないようにすることが重要である。

<!-- ## Supporter -->

## サポーター {#supporter}

<!-- Supporter is a specific Stakeholder type. Supporters are supporting Stakeholders and change agents. Supporters are often part of a powerful guiding coalition [45], who inspire and remove demotivating factors. Supporters support the Scrum Team to thrive and influence the organization's workflows, processes, systems, Products, services, and work environment to become coherent with a Scrum adoption and emergence [21]. Supporters should participate when and where needed or as requested. Value creation often requires effective and constructive collaboration with other Stakeholders. -->

サポーターは特定のステークホルダータイプである。サポーターは支援するステークホルダーでありチェンジエージェントである。サポーターはしばしば強力な指導連合[45]の一部であり、インスピレーションを与え、やる気をそぐ要因を取り除く。サポーターは、スクラムチームが繁栄することを支援し、組織のワークフロー・プロセス・システム・プロダクト・サービス・作業環境がスクラム適用と創発[21]と一貫するよう影響を与える。サポーターは必要な時と場所で、または要求に応じて参加すべきである。価値創造はしばしば他のステークホルダーとの効果的で建設的なコラボレーションを必要とする。

<!-- Depending on the size of the organization, examples of Supporters include (but are not limited to) colleagues, decision-makers, financial sponsors, governance oversight, managers, subject matter experts, marketing, HR, finance, procurement, and early adopters. Supporters who do not empower Scrum Teams to do what is recommended in this document are not really Supporters. Executives and board members have a crucial role in fostering a climate where Supporters support. Supporters should demonstrate leadership that the Scrum Team appreciates. -->

組織の規模に応じて、サポーターの例には、同僚、意思決定者、資金提供者、ガバナンス監督、マネージャー、特定分野のエキスパート、マーケティング、HR、財務、調達、アーリーアダプターが含まれる（ただしこれらに限定されない）。この文書で推奨されることをスクラムチームができるようにエンパワーメントしないサポーターは、サポーターとはいえない。経営層と役員は、サポーターが支援できる環境を育むうえで、重要な役割を持つ。サポーターは、スクラムチームにとって価値のあるリーダーシップを発揮すべきである。

<!-- ## Artificial Intelligence -->

## 人工知能 {#artificial-intelligence}

<!-- Artificial Intelligence (AI) is increasingly part of the work environment and may significantly expand a Scrum Team's capabilities in discovery, decision-making, Product development, and value realization. -->

人工知能（AI）はますます作業環境の一部となり、ディスカバリー、意思決定、プロダクト開発、価値実現におけるスクラムチームの能力を大幅に拡張する可能性がある。

<!-- AI may enhance Scrum through:

- Empirical Process Control [27-29]: AI-driven analytics improve transparency, inspection, and adaptation.
- Cognitive Augmentation: AI allows human Scrum Team members to focus on strategic, creative, and ethical considerations.
- Continuous Value Adaptation: AI could update and reprioritize Product Backlog Items informed by live user feedback and trends.
- Systems Insight: AI identifies hidden interdependencies, improving data-informed decision-making. -->

AIは以下を通じてスクラムを強化する可能性がある：

- 経験的プロセス制御[27-29]：AI駆動の分析により、透明性・検査・適応が改善される。
- 認知的拡張：AIにより、人間のスクラムチームメンバーは戦略的・創造的・倫理的な検討に集中できる。
- 継続的な価値適応：AIは、リアルタイムのユーザーフィードバックとトレンドに基づき、プロダクトバックログアイテムの更新と再優先順位付けを行うことができる。
- システム洞察：AIは隠れた相互依存関係を特定し、データに基づいた意思決定を改善する。

<!-- The dangers are endless. Maintain clear human accountability for all outcomes (guided by the accountabilities from Scrum), using AI as a powerful but supervised decision-making partner. This is known as keeping the 'human in the loop.' While AI can enhance innovation and effectiveness at the lowest costs, it does not replace human accountability. AI should support—not override—Scrum's empirical process control [27-29] and ethical [30] decision-making. The Scrum Team remains accountable for delivering valuable outcomes, assessing evidence, and upholding professionalism. -->

危険もまた、無限にあるものだ。すべてのアウトカムに対して、人間に説明責任があることを明確に維持した上で（スクラムにおける説明責任に従う）、強力だが監督された意思決定パートナーとしてAIを使う。これは「ヒューマン・イン・ザ・ループ」として知られている。AIによって、最小のコストでイノベーションと効果性を高めることができる。しかし、人間の説明責任を置き換えることはできない。AIはスクラムにおける経験的プロセス制御[27-29]と倫理的[30]意思決定を支援すべきであり、上書きしてしまってはならないのだ。スクラムチームは、価値あるアウトカムの提供・エビデンスの評価・プロフェッショナリズムを守ることに対して、引き続き説明責任を負う。

<!-- The possibilities are also endless. Scrum Teams could leverage AI to:

- Improve Product Backlog Refinement.
- Discover ambiguities in text and continuously inspect its own recommendations and results for bias, errors, and unintended consequences.
- Regularly validate and adapt models and applications.
- Foster transparency in Product Backlog ordering (sequencing).
- Create agents as AI team members.
- AI can be helpful to deliberately test and challenge the existing thinking. -->

可能性もまた無限である。スクラムチームは以下のためにAIを活用できる：

- プロダクトバックログリファインメントを改善する。
- テキスト内の曖昧さを見つけ出し、自らの推奨や結果に偏り、誤り、意図しない結果が含まれていないかを継続的に検査する。
- モデルとアプリケーションを定期的に検証し適応させる。
- プロダクトバックログの順序付け（シーケンス化）における透明性を促進する。
- AIチームメンバーとしてエージェントを作成する。
- AIは既存の思考を意図的にテストし挑戦するのに役立つ。

<!-- AI can be a supporting tool if used with good intent. AI tools should be evaluated like any other contributor to psychological flow [46] and learning: Do they improve feedback loops? Do they help validate assumptions faster? Do they act, and when they do, is it ethical [30] action? -->

AIは善意に基づいて使用されれば、人を支援するツールになりうる。AIツールは、他の貢献者を評価する際と同様に心理学的フロー[46]や学習において、評価されるべきである。フィードバックループを改善するだろうか？仮説をより迅速に検証するのに役立つだろうか？行動するだろうか？行動するならば、倫理的[30]な行動といえるだろうか？

<!-- Psychological flow [46] is a state of complete absorption and enjoyment in an activity, where action and awareness merge, and time seems to pass differently. -->

心理学的フロー[46]は、活動への完全な没頭と楽しみの状態であり、行動と認識が融合し、時間が異なって過ぎるように見える。

<!-- Scrum encourages the Scrum Team to experiment with AI responsibly using small, sometimes reversible trials. Adaptation and inspection apply not only to the Product but also to how AI is integrated into delivery. -->

スクラムは、スクラムチームが小さく、時には可逆的な試行を使用してAIを責任を持って実験することを奨励する。適応と検査は、プロダクトだけでなく、AIが提供にどのように統合されるかにも適用される。

<!-- The focus should remain on the human dynamics of teamwork and collaboration, with AI positioned as a potential aid to attain adaptiveness at speed. -->

焦点は、チームワークとコラボレーションの人間の力学に留まるべきであり、AIはスピードを伴う適応性の獲得を支援する潜在的な手段として位置付けられる。

<!-- ## Product Developer -->

## プロダクト開発者 {#product-developer}

<!-- Product Developer is a role and an accountability. All Product Developers together should possess all the skills needed to create Increments. The combined skill set is often referred to as cross-functional. -->

プロダクト開発者は役割および説明責任の一つである。すべてのプロダクト開発者はインクリメントを作成するために必要な一通りのスキルを合わせ持つべきである。これらのスキルセットは機能横断型とよく呼ばれる。

<!-- A Product Developer may be human or automated. Human Product Developers are _Committed_ to creating, researching, inspecting, and adapting any aspect of a releasable Increment each Sprint. Their primary _Focus_ is on the current Sprint. Some capacity is often invested into future-looking refinement and examining result feedback, side effects, or other learning. -->

プロダクト開発者は人間でも自動化された存在でもよい。人間のプロダクト開発者は、リリース可能なインクリメントのあらゆる側面をスプリント毎に作成、調査、検査、適応することを _確約_ している。彼らの主な _集中_ は現在のスプリントにある。ただし、プロダクト開発者の一部のキャパシティは将来に向けたリファインメントや、結果からのフィードバック（結果フィードバック）、副次的影響、その他の学習の検査に投資されることが多い。

<!-- Product Developers adhere to the Definition of Output Done and strive for net improvement. The Product Developers achieve the best results if they _Focus_ solely on one Product. If, at a given point in time, the Product Owner or Scrum Master actively works on items in the Sprint Backlog, they perform that work as Product Developers. -->

プロダクト開発者はアウトプット完成の定義を遵守し、実質的な改善を目指す。プロダクト開発者は、1つのプロダクトに _集中_ することで最良の結果を達成する。ある時点でプロダクトオーナーまたはスクラムマスターがスプリントバックログのアイテムに対する作業に取り組む場合、その作業はプロダクト開発者として実行する。

<!-- The Product Developers should adopt appropriate behaviors depending on the situation; these include (but are not limited to) collaborator, creator, and a champion of technical quality, discovery, delivery, and value validation. -->

プロダクト開発者は状況に応じて適切な行動を取る必要がある。例えば、協力者、クリエイター、技術的品質、探索、デリバリー、価値検証の推進者として行動するなどがあるが、これらに限定されない。

<!-- _At least one Product Developer should be human._ Multiple human Product Developers often improve cognitive diversity, helpful for addressing complexity. -->

_少なくとも1人のプロダクト開発者は人間であるべきである。_ 複数の人間のプロダクト開発者は多くの場合に認知的多様性を向上させ、複雑性への対応に役立つ。

<!-- Product Developers are always collectively accountable for:

- Creating an emergent plan in the Sprint Backlog for achieving the Sprint Goal;
- Instilling quality by adhering to and improving the Definition of Output Done;
- Creating at least one usable Increment every Sprint;
- Learning, often through data that is guided by the Definition of Outcome Done;
- Adapting their plan each day toward the Sprint Goal;
- Holding each other accountable as professionals; and,
- Net improvement. -->

プロダクト開発者は常に以下に対して集合的に説明責任を負う：

- スプリントゴール達成のための創発的な計画をスプリントバックログ内で作成する
- アウトプット完成の定義を遵守し改善することで品質を作り込む
- 毎スプリント少なくとも1つの使用可能なインクリメントを作成する
- アウトカム完成の定義により導かれるデータなどを通じて学習する
- スプリントゴールに向けて日々計画を適応させる
- プロフェッショナルとしてお互いに責任を負う
- 実質的な改善

<!-- Context matters, it is crucial to consider the specific circumstances. But as a rule of thumb, a Product Developer who is neither willing nor ready nor able to be a professional should step down as a Product Developer. -->

文脈は重要であり、その場で起きている特定の状況を考慮することが重要である。しかし経験則として、プロフェッショナルとしての意志、準備、能力がないプロダクト開発者は、その役割から退くべきである。

<!-- ## Product Owner -->

## プロダクトオーナー {#product-owner}

<!-- Product Owner is a role and an accountability. The Product Owner must be human. To be effective, the Product Owner should be a leader for the Product. The Product Owner maximizes long-term value and needs to know where the value is and when it is needed. The Product Owner is expected to work at all levels and across all relevant business areas. The Product Owner collaborates with Stakeholders, the Scrum Master, and the Product Developers to create value. -->

プロダクトオーナーは役割および説明責任の一つである。プロダクトオーナーは人間でなければならない。効果的であるために、プロダクトオーナーはプロダクトのリーダーであるべきである。プロダクトオーナーは長期価値を最大化し、価値がどこにあり、いつ必要かを知る必要がある。プロダクトオーナーは、すべてのレベルおよび関連するすべてのビジネス領域において業務を行うことが求められる。プロダクトオーナーは、ステークホルダー・スクラムマスター・プロダクト開発者と協働して価値を創出する。

<!-- The Product Owner uses the Product Backlog to define what gets built and in what approximate order. The Product Owner always keeps the Product Goal in mind; their primary _Focus_ is to maximize long-term value at every step. -->

プロダクトオーナーは、プロダクトバックログを用いて、何を構築するか、そしておおよそどの順序で構築するかを定義する。プロダクトオーナーは常にプロダクトゴールを念頭に置いており、主要な _集中_ は、あらゆる段階で長期的な価値を最大化することである。

<!-- The Product Owner is not defined by analyzing and writing detailed Product Backlog Items. Every minute spent not trusting the Product Developers is a missed chance to think more strategically, work more with Stakeholders, or create more value. The Product Owner should adopt appropriate behaviors depending on the situation; these include (but are not limited to) being a visionary, customer representative, collaborator, influencer, experimenter, decision maker, and champion of Stakeholder engagement, clarity, Product quality, and value realization. -->

プロダクトオーナーは、詳細なプロダクトバックログアイテムの分析と記述によって定義されるものではない。プロダクト開発者を信頼せずに細かく管理・監督することに費やす分だけ、より戦略的に思考し、よりステークホルダーと連携し、より価値を生み出すための機会が奪われるのである。プロダクトオーナーは状況に応じて適切な行動を取るべきであり、それにはビジョナリー、顧客代表、協力者、影響者、実験者、意思決定者、そしてステークホルダーエンゲージメント・明確性・プロダクト品質・価値実現の推進者などが含まれる（ただしこれらに限定されない）。

<!-- The Product Owner is always accountable for:

- Stakeholder engagement, understanding Stakeholders, their power, expectations, needs, and wants;
- Continuously sensing, listening, learning, and adapting as needed;
- Continuously balancing trade-offs, including but not limited to:
  - Quality, speed, capability, risk reduction, value, simplicity [47];
  - Stakeholders and their multiplicity of often competing expectations and limits;
  - Value, work climate (sustainability of the Scrum Team is important), potential customers;
- Developing and explicitly communicating the Product Goal;
- Developing and effectively communicating a coherent Product narrative;
- Creating and clearly communicating Product Backlog Items;
- Ordering Product Backlog Items;
- Ensuring that the Product Backlog is transparent and understood;
- Effectively communicating outcomes supported by measures in the Definition of Outcome Done;
- Having the final say on the Definition of Outcome Done;
- Fostering the high-quality creation, discovery, delivery, and validation of value; and,
- Other Product management activities as required. -->

プロダクトオーナーは常に以下に対して説明責任を負う：

- ステークホルダーエンゲージメント・ステークホルダーとその権力・期待・ニーズ・要望の理解
- 必要に応じた継続的な感知・傾聴・学習・適応
- 以下の事項（ただしこれらに限定されない）においてトレードオフのバランスを取り続けること：
  - 品質・速度・ケイパビリティ・リスク削減・価値・シンプルさ[47]
  - ステークホルダー・しばしば相反する複数の期待と制約
  - 価値・作業風土（スクラムチームの持続可能性は重要である）・潜在顧客
- プロダクトゴールを策定し、それを明確に伝えること
- 一貫性のあるプロダクトのナラティブを構築し、それを効果的に伝えること
- プロダクトバックログアイテムの作成と明確なコミュニケーション
- プロダクトバックログアイテムの並び替え
- プロダクトバックログの透明性が高く、関係者に正しく理解されることの保証
- アウトカム完成の定義において、計測指標に基づくアウトカムを効果的に伝えること
- アウトカム完成の定義に対する最終決定権
- 高品質な価値の創造・ディスカバリー・デリバリー・検証の促進
- 必要に応じた他のプロダクトマネジメント活動

<!-- The Product Owner may do the above work or collaborate with the Scrum Team to mutually agree on responsibilities for doing the above work. Regardless, the Product Owner remains accountable. -->

プロダクトオーナーは、上記の作業を自ら実施することもできるし、スクラムチームと協力してその作業に関する責任を相互に合意することもできる。いずれにしても、プロダクトオーナーが説明責任を負う。

<!-- For Product Owners to succeed, all Stakeholders and Supporters should _Respect_ their decisions. These decisions are visible in the content and ordering of the Product Backlog and through the inspectable Increment at the Sprint Review. The Product Owner has delegated authority from the organization. -->

プロダクトオーナーが成功するためには、すべてのステークホルダー・サポーターは、その意思決定を _尊敬_ すべきである。これらの意思決定は、プロダクトバックログの内容・順序・スプリントレビューで検査可能なインクリメントを通じて可視化される。プロダクトオーナーは組織から権限を委譲されている。

<!-- Product Ownership requires strong Product management skills and domain skills. A Product Owner lacking these skills may need support and guidance until they develop the necessary expertise. Context matters. But as a rule of thumb, a Product Owner who is neither willing, ready, nor able to gain Product management skills should step down as Product Owner. A domain subject matter expert is not necessarily the best choice for a Product Owner as Product management skills and leadership are needed; for example, the Product Developer accountability is often more appropriate. -->

プロダクトオーナーシップには、優れたプロダクトマネジメントスキルおよびドメインに関するスキルが求められる。これらのスキルを欠くプロダクトオーナーは、必要な専門性を身につけるまでの間、支援とガイダンスを受ける必要がある。文脈は重要である。しかし経験則として、プロダクトマネジメントスキルを身につける意思・準備・能力のいずれも持たないプロダクトオーナーは、その職務を辞するべきである。特定分野のエキスパートが、必ずしもプロダクトオーナーに最適であるとは限らない。なぜなら、プロダクトマネジメントスキルとリーダーシップが求められるためである。例えば、プロダクト開発者の方が適切である場合も多い。

<!-- If the Scrum Team inadvisably works on multiple Products, platforms, or projects, each Product, platform, or project manager should be a Stakeholder (and Supporter) of the Product Owner and collaborate to maximize long-term value. Scrum encourages the Scrum Team to stay _Focused_ and _Committed_, helping it deliver valuable outcomes and avoid the pitfalls associated with operating as a 'feature-factory.' -->

スクラムチームが不適切に複数のプロダクト、プラットフォーム、またはプロジェクトに取り組む場合、各プロダクト、プラットフォーム、またはプロジェクトのマネージャーはプロダクトオーナーのステークホルダー（およびサポーター）となり、長期的な価値を最大化するために協力する必要がある。スクラムはスクラムチームが _集中_ と _確約_ を維持することを奨励し、価値あるアウトカムを届け、「フィーチャーファクトリー」として運営するリスクを回避することを支援する。

<!-- The Product Owner is one person, not a committee or technology. Those wanting to change the Product Backlog need to convince the Product Owner. The Product Owner maximizes long-term value and often makes trade-offs in doing so. -->

プロダクトオーナーは一人の人間であり、委員会やテクノロジーではない。プロダクトバックログを変更したい人は、プロダクトオーナーを説得する必要がある。プロダクトオーナーは長期的な価値を最大化し、その過程でしばしばトレードオフを行う。

<!-- ## Scrum Master -->

## スクラムマスター {#scrum-master}

<!-- The Scrum Master is a role and an accountability. The Scrum Master must be human. The Scrum Master is a change agent who works at all organizational levels and across business areas. The Scrum Master leads by example and guides the effectiveness of the Product Owner, Scrum Team, Stakeholders, and Supporters in their adoption of Scrum. The Scrum Master understands complexity [12-17] and is skillful in enabling the next right thing. -->

スクラムマスターは役割および説明責任の一つである。スクラムマスターは人間でなければならない。スクラムマスターはチェンジエージェントであり、組織全体のあらゆるレベルや事業領域で活動する。スクラムマスターは模範を示してリードし、プロダクトオーナー、スクラムチーム、ステークホルダー、サポーターがスクラムを適用する際の効果性を高めるよう導く。スクラムマスターは複雑性[12-17]を理解し、次の正しい行動を可能にするスキルを備える。

<!-- The Scrum Master should adopt appropriate behaviors depending on the situation; these include (but are not limited to) being a guide, coach, mentor, teacher, observer, impediment remover, agent of change, effectiveness facilitator, and continuous improvement champion. The Scrum Master is neither a team administrator, status manager, taskmaster, rule-dictator, meeting-room booker, report dashboard administrator, chairperson, hero, coordinator, nor an in absentia Scrum Master, leaving everything to 'self-management.' -->

スクラムマスターは状況に応じて適切に振る舞う必要がある。これにはガイド、コーチ、メンター、教師、観察者、障害物除去者、チェンジエージェント、効果性のファシリテーター、継続的改善の推進者などが含まれるが、これらに限定されない。一方でスクラムマスターはチーム管理者、進捗管理者、タスク指示者、ルール決定者、会議室予約係、レポートやダッシュボードの管理者、議長、ヒーロー、調整役ではなく、すべてをチームの「自己管理」に任せて不在のスクラムマスターでもない。

<!-- The Scrum Master is accountable for the effectiveness of the Scrum Team, Stakeholders, Supporters, and the affected people in embracing empiricism [19], self-management, and Scrum adoption as described in this document. The Scrum Master addresses whatever impedes or slows a Scrum Team's progress and cannot be resolved by the Scrum Team. -->

スクラムマスターは、スクラムチーム・ステークホルダー・サポーター・影響を受ける人々が、本文書で説明されている経験主義[19]・自己管理・スクラム適用の効果性を高めることに説明責任を負う。スクラムマスターはスクラムチームが解決できない、進捗を阻害したり遅らせたりするあらゆる障害物の除去に取り組む。

<!-- The Scrum Master supports the Scrum Team, Product Owner, and Supporters in several ways, including: -->

スクラムマスターは、さまざまな形でスクラムチーム、プロダクトオーナー、サポーターを支援する：

<!-- - Helping everyone understand Scrum theory and practice, educating or coaching when needed;
- Enabling the Scrum Team and Supporters to improve in a variety of ways continuously;
- Fostering timely, purposeful, and intentional interactions;
- Ensures the Scrum Team has a suitable Definition of Output Done;
- Ensuring that all Scrum events take place and are constructive, productive, and kept within the relevant time limit;
- Causing the removal of impediments to Product-related work and to effective Scrum adoption;
- Coaching toward self-management [11] and cross-functionality;
- Helping the Scrum Team, Stakeholders, and Supporters understand their importance in supporting high-value Increments that meet the Definition of Output Done toward the Product Goal and Definition of Outcome Done;
- Improving adaptiveness [37] and optimizing the flow of value;
- Fostering evidence-informed confidence but being compassionate and timely to avoid overconfidence;
- Fostering change agency and general agency by the Scrum Team and Supporters;
- Encouraging helpful behaviors within the Scrum Team that are aligned with the Scrum Values to foster trust, collaboration, and high performance; and,
- Fostering the Scrum Team to deliver valuable work, get feedback, and do rework as needed, quickly and often. -->

- 全員がスクラムの理論と実践を理解できるよう支援する。そのために必要に応じて教育やコーチングを行う
- スクラムチームとサポーターが様々な方法で継続的に改善できるよう支援する
- タイムリーで意図的な目的を持った相互作用を促進する
- スクラムチームが適切なアウトプット完成の定義を持てるよう努める
- すべてのスクラムイベントが実施され、建設的かつ生産的であり、関連する時間制限内で完了するようにする
- プロダクトに関連する作業や効果的なスクラム適用を阻害する障害物を取り除く
- 自己管理[11]と機能横断な行動に向けたコーチング
- プロダクトゴールおよびアウトカム完成の定義の実現に向かうために、アウトプット完成の定義を満たす価値の高いインクリメントの作成をスクラムチーム、ステークホルダー、サポーターがサポートすることの重要性を理解できるように支援する
- 適応性[37]を改善し、フロー（価値の流れ）を最適化する
- エビデンスに基づく自信を育みながらも、過信を避けるために相手の気持ちに共感しタイムリーであろうとする
- スクラムチームやサポーターがチェンジエージェントとして振る舞い、あらゆることに主体的に行動するよう促す
- 信頼、コラボレーション、高パフォーマンスを促進するスクラムの価値基準に沿ってスクラムチームが効果的に行動することを支援する
- スクラムチームが価値ある作業を提供し、フィードバックを得て、必要に応じて迅速かつ頻繁に再作業をできるようにする

<!-- The Scrum Master supports the Scrum Team in several ways, including: -->

スクラムマスターは、さまざまな形でスクラムチームを支援する：

<!-- - Supporting the Scrum Team in its formation, upskilling, and continuous improvement;
- Helping the Scrum Team understand the need for clear and concise Product Backlog Items that deliver value; and,
- Being vigilant that the entire Scrum Team is collaborating purposefully and intentionally with each other and Stakeholders, honoring the Definition of Output Done, and focused on creating high-value Increments according to the Definition of Outcome Done. -->

- スクラムチームの立ち上げ、スキル向上、継続的改善を支援する
- 価値を提供する明確で簡潔なプロダクトバックログアイテムの必要性についてスクラムチームに理解してもらう
- スクラムチーム全体が互いに、そしてステークホルダーと意図的かつ目的を持って協力し、アウトプット完成の定義を尊重し、アウトカム完成の定義に沿って価値の高いインクリメントを作成することに集中できるよう常に意識を向ける

<!-- The Scrum Master supports the Product Owner in several ways, including: -->

スクラムマスターは、さまざまな形でプロダクトオーナーを支援する：

<!-- - Helping find techniques for effective Product Goal definition and Product Backlog management;
- Helping establish emergent Product planning for a complex [12-17] environment;
- Helping the Product Owner to express outcomes as measures through the Definition of Outcome Done;
- Helping the Product Owner understand the need for clear and concise Product Backlog Items that deliver value; and,
- Helping the Product Owner to Focus on value realization. -->

- 効果的なプロダクトゴールの定義とプロダクトバックログ管理の⽅法を探すことを支援する
- 複雑な[12-17]環境における創発的なプロダクト計画の策定を支援する
- アウトカム完成の定義に沿って計測されたアウトカムをプロダクトオーナーが表現できるようにする
- 価値を提供する明確で簡潔なプロダクトバックログアイテムの必要性についてプロダクトオーナーに理解してもらう
- プロダクトオーナーが価値実現に _集中_ できるよう支援する

<!-- The Scrum Master supports the Stakeholders in several ways, including: -->

スクラムマスターは、さまざまな形でステークホルダーを支援する：

<!-- - When more than expertise is needed, helping affected people and Stakeholders understand and adopt:
  - An empirical approach for complex [12-17] work where cause and effect are only coherent in retrospect,
  - Going beyond empirical process control, e.g., running multiple parallel safe-to-fail experiments, seeking fresh thinking, exaptation, or testing educated hunches. Exaptation means taking something that was made or used for one purpose and using it for a different purpose, especially when facing new or unclear situations.
- Fostering actions that support the mantra 'Stop putting items in progress; start finishing items;'
- Facilitating Stakeholder collaboration as requested or needed;
- Helping Stakeholders understand the need for clear and concise Product Backlog Items that deliver value; and,
- Helping the Stakeholders to _Focus_ primarily on value realization. -->

- 専門知識を超える取り組みが必要なとき、影響を受ける人やステークホルダーが以下を理解し採用することを手助けする：
  - 後から振り返ってはじめて因果関係が明らかになるような、複雑な[12-17]仕事における経験主義的アプローチ
  - 経験的プロセス制御の枠を超えたアプローチ。例えば、安全に失敗できる実験の複数並行した実行、新たな思考の追求、外適応、経験的な直感の試行。外適応（exaptation）とは、ある目的のために作成または使用されたものを、新たな状況や不透明な状況において、異なる目的に使用すること
- 「アイテムを仕掛中にするのはやめ、完成させる活動を始めよう」というモットーに沿う行動を促進する
- 要求・必要に応じて、ステークホルダーのコラボレーションを促進する
- 価値を提供する、明確で簡潔なプロダクトバックログアイテムの必要性についてステークホルダーの理解を手助けする
- ステークホルダーが価値実現に最も _集中_ できるよう手助けする

<!-- The Scrum Master works with the Supporters in several ways, including: -->

スクラムマスターは、さまざまな形でサポーターと協働する：

<!-- - Leading, training, and coaching the Supporters in the Scrum adoption;
- Clarifying what is getting in the way of an effective Scrum adoption;
- Facilitating disciplined emergent change in a direction to support the Scrum adoption; and,
- Fostering organizational changes toward ease of delivery vs ease of management. -->

- スクラム適用においてサポーターに対し指導・トレーニング・コーチする
- 効果的なスクラムの適用を阻害している要因を明確にする
- スクラム適用を支援する方向への規律ある創発的変化を促進する
- 管理の容易さからデリバリーの容易さを重視する組織への変革を促進する

<!-- The Scrum Master works with the organization in several ways, including: -->

スクラムマスターは、さまざまな形で組織と協働する：

<!-- - Leading, training, and coaching the organization in its Scrum adoption(s);
- Planning and advising Scrum adoptions within the organization;
- Working with related departments in how they could support the Scrum adoption; and,
- Removing barriers to the Scrum adoptions. -->

- 組織へのスクラム適用を指導・トレーニング・コーチする
- 組織内のスクラム適用計画を策定し助言する
- 関連部署とスクラム適用を支援する方法について協議する
- スクラムの適用を妨げる障害物を取り除く

<!-- Scrum Masters can team up with other Scrum Masters or Supporters to support the whole organization; they can also collaborate with other change agents or leaders when needed. The Scrum Master, as a change agent, is accountable for the quality of the Scrum adoption and should collaborate with other change agents to improve it. -->

スクラムマスターは組織全体を支援するために他のスクラムマスターやサポーターとチームを組むことができる。必要に応じて他のチェンジエージェントやリーダーと協力することもできる。スクラムマスターはチェンジエージェントとしてスクラム適用の品質に説明責任を負い、その品質を改善するために他のチェンジエージェントと協力して進めるべきである。

<!-- The Scrum Master is one person, not a committee or technology, and serves the Product Owner, Scrum Team, Stakeholders, and the larger organization. Being a change agent and leader, the Scrum Master should generally invite people to participate in the change. It is helpful if the Scrum Master has an understanding of the flow of value [48-49], lean [20], complexity theory [12-17], and other supporting and complementary theory in this document, as well as assisting people with the _how_. It is also helpful if the Scrum Master is unrelenting and has an insatiable appetite for learning and change. -->

スクラムマスターは1人の人間であり、委員会や技術ではない。スクラムマスターはプロダクトオーナー、スクラムチーム、ステークホルダー、より大きな組織に奉仕する。チェンジエージェントかつリーダーであり、一般的に人々を変革へ参加するよう招待すべきである。スクラムマスターが価値の流れ[48-49]、リーン[20]、複雑性理論[12-17]、そしてこの文書に記載されたその他の支援的・補完的理論を理解し、どのように（_How_）行動すべきかを人々に示すことが望ましい。粘り強く、学びと変化への飽くなき欲求を持っていることもスクラムマスターに求められる素養である。

<!-- Being a Scrum Master is a calling where helping others succeed is reward enough. A Scrum Master doesn't seek the spotlight. Like any good leader, they give credit to others and take responsibility when things go wrong. Staying in the role for a longer time helps guide the Scrum Team toward its full potential, but only if the Product Developers collectively develop self-management. Parent-style Scrum Master behavior does not foster a self-managing Scrum Team. Context matters. But as a rule of thumb, a Scrum Master who is neither willing, ready, nor able to be an agent of change should step down as a Scrum Master. -->

スクラムマスターは、他者の成功に貢献することを大きなやりがいとする役割である。スクラムマスターは目立とうとはしない。優れたリーダーと同様に、功績を他者に譲り、物事がうまくいかない時には責任を取る。長期的にスクラムマスターを務めることでスクラムチームの潜在能力を最大限引き出すことができるが、それはプロダクト開発者がチームとして自己管理を身につけた場合に限る。親のようなスクラムマスターの振る舞いは自己管理スクラムチームの成長を妨げる。文脈は重要だが、経験則として、変革の担い手となる意志、準備、能力がないスクラムマスターはその役割から退くべきである。

<!-- ## The Scrum Artifacts in the Expansion Pack -->

## 拡張パックにおけるスクラムの作成物 {#the-scrum-artifacts-in-the-expansion-pack}

<!-- Scrum's artifacts provide Transparency about what the Scrum Team and Stakeholders believe will deliver value. Thus, everyone can have the same basis for Inspection and Adaptation. -->

スクラムの作成物は、スクラムチームとステークホルダーが価値を生み出すと信じている内容について、透明性をもたらす。これにより、誰もが同じ基準で作業内容を検査し、必要に応じて適応できるようになる。

<!-- Each artifact contains a commitment:

- For the Product serving the Stakeholders, it is the Definition of Outcome Done. (SGEP added)
- For the Increment that is a candidate update for the Product, it is the Definition of Output Done (SGEP renamed).
- For the Product Backlog, it is the Product Goal.
- For the Sprint Backlog, it is the Sprint Goal. -->

また、各作成物には「確約（コミットメント）」が含まれている：

- ステークホルダーに提供するプロダクトについては、アウトカム完成の定義（SGEP追加）
- プロダクトのアップデート候補であるインクリメントについては、アウトプット完成の定義（SGEP改名）
- プロダクトバックログについては、プロダクトゴール
- スプリントバックログについては、スプリントゴール

<!-- Upon release of the Increment (output), the Product is what creates value (outcomes). Value is the measurable or observable fulfillment or creation of expectations, needs, or wants from the Stakeholders' perspective. -->

インクリメント（アウトプット）がリリースされることで、プロダクトが価値（アウトカム）を生み出すことになる。ここでいう価値とは、計測可能または観察可能な形で、ステークホルダーの視点から見た、期待やニーズ、要望が満たされたり、新たに生み出されたりすることである。

<!-- These commitments reinforce the pillars of Transparency, Inspection, and Adaptation, enabling empirical process control [27-29]. The Product Goal is fixed for as long as no contrary evidence or observations emerge in the observed Product's Definition of Outcome Done. The Definition of Output Done is not weakened during the Sprint. So what could be changed instead? It could be the Acceptance Criteria for a specific Product Backlog Item, the implementation or fidelity of a specific feature, or even alternative Product Backlog Items for achieving the Sprint Goal, etc. -->

これらのコミットメントは、透明性・検査・適応というスクラムの三本柱を強化し、経験的なプロセス制御を可能にする[27-29]。プロダクトゴールは、プロダクトのアウトカム完成の定義において反対のエビデンスや観察が現れない限り、固定される。アウトプット完成の定義はスプリント中に妥協されることはない。では、代わりに何が見直されたり変更されたりするのかというと、例えば、特定のプロダクトバックログアイテムの受け入れ基準や、特定の機能の実装内容や精度、あるいはスプリントゴール達成のための代替となるプロダクトバックログアイテムなどが挙げられる。

<!-- If the Product Goal shifts often, it could indicate that something is off, perhaps due to a lack of Focus on what matters. Focus is about being professional and deciding what to work on but also what not to work on. -->

もしプロダクトゴールが頻繁に変わるようであれば、それは何かがうまくいっていない兆候を示しており、重要なことに _集中_ できていない可能性がある。_集中_ とは、プロフェッショナルとして何に取り組むかだけでなく、何に取り組まないかを決めることでもある。

<!-- ## Product -->

## プロダクト {#product}

<!-- The Product is an artifact. A Product can be a holistic experience or a platform. It can also be a service, physical, digital, or hybrid, delivering continuous value to Stakeholders (including but not limited to users). -->

プロダクトは作成物の一つである。プロダクトは包括的な体験またはプラットフォームとなることができる。また、サービス、物理的、デジタル、またはハイブリッドであり、ステークホルダー（ユーザーを含むがこれに限定されない）に継続的な価値を提供する。

<!-- An experience is a specific solution designed to meet the needs of Stakeholders, including the user, ideally external to the organization. It provides a direct interaction that delivers value. It is typically focused on solving a particular problem or opportunity, or a set of them for Stakeholders, including but not limited to customers, decision-makers, and users. -->

体験とは、理想的には組織外のユーザーを含むステークホルダーのニーズを満たすように設計された特定のソリューションである。それは価値を提供する直接的な相互作用を提供する。ステークホルダーの特定の課題や機会、またはそれらの組み合わせを解決することに焦点を当てている。対象となるステークホルダーには、顧客、意思決定者、ユーザーなどが含まれるがそれらに限定されない。

<!-- A platform is an architectural device, foundational infrastructure, or set of tools that enables developers to build Products in order to provide an experience. Platforms provide a base for multiple Products to be developed upon, focusing on scalability, reliability, and flexibility for engineers rather than direct user interaction. -->

プラットフォームとは、体験を提供するためのプロダクトを開発者が構築することを可能にするアーキテクチャデバイス、基盤となるインフラストラクチャ、またはツールセットである。プラットフォームは複数のプロダクトを構築するための基盤を提供し、直接的なユーザーとの相互作用よりもエンジニアのためのスケーラビリティ、信頼性、柔軟性に重点を置く。

<!-- The Scrum Team and Stakeholders need to have a clear understanding at all times of what the Product is, who the customers, users, or decision-makers are, and the type of Product it is —like one for end-users, employees, or Scrum Teams—has different Stakeholders and ways it creates value. A Product is evolutionary and often long-lived. The Product needs a single Product Backlog to increase Transparency and maximize value. -->

スクラムチームとステークホルダーはこのプロダクトが何であるか、顧客、ユーザー、または意思決定者が誰であるか、そしてどのようなタイプのプロダクトなのか（エンドユーザー向け、従業員向け、スクラムチーム向けなど）を常に明確な理解を持つ必要がある。プロダクトのタイプにより異なるステークホルダーが存在し、価値創出の方法も異なることを理解する必要がある。プロダクトは進化的であり、しばしば長期にわたり存続する。透明性を高め、価値を最大化するために、プロダクトには単一のプロダクトバックログが必要である。

<!-- Context matters. But as a rule of thumb, for a Product to create and maintain traction, it helps if the Product:

- Sufficiently addresses satisfaction gaps;
- Is valuable, desirable, viable, usable, feasible, safe, and secure;
- Has professionalism built-in;
- Has a compelling, clear, and outcome-metric-oriented Product Vision, Product strategy, and Product Goal, often including intent, rationale, and anti-goals;
- Adapts and improves to identify, represent, or measure emergence [21]; and,
- Is extendable and maintainable. -->

文脈は重要である。しかし、経験則として、プロダクトが牽引力を生み出し、それを維持するためには、以下の条件を満たすことが有効である：

- 満足度のギャップに十分に対処している
- 価値があり、望ましく、実行可能で、使用可能で、実現可能で、安全で、セキュアである
- プロフェッショナリズムが組み込まれている
- 明確で説得力があり、成果指標に基づくプロダクトビジョン、プロダクト戦略、プロダクトゴールを備えている。その中には意図、根拠、避けるべきゴールが含まれる事が多い
- 創発[21]を特定、表現、評価するために適応し改善する
- 拡張可能であり、保守可能である

<!-- The Product is the manifestation of _why_ we do _what_ we do. -->

プロダクトは、我々が何のために仕事をしているのかを表現したものである。

<!-- ## Commitment: Definition of Outcome Done -->

## コミットメント：アウトカム完成の定義 {#commitment-definition-of-outcome-done}

<!-- The Definition of Outcome Done is a commitment. It describes the observable evidence measures (quantitative or qualitative) required to demonstrate realized benefits, often referred to as value validation. It could be for the overall Product or a specific goal. It's often best to define the measures for value validation before realization starts, as this avoids biases and mistaken interpretations. -->

アウトカム完成の定義はコミットメントの一つである。これは、実現された価値を示すために必要な観察可能なエビデンスの計測基準（定量的または定性的）を記述し、しばしば価値検証と呼ばれる。これはプロダクト全体、または特定のゴールに対して設定される。バイアスや誤った解釈を避けるため、実装を開始する前に価値検証のための計測基準を定義しておくことが最善であることが多い。

<!-- Outcomes confirm user changes; impact confirms organizational results. Together with related interpretations they inform future adaptations, ideally confirming the intended business impact. It could be for a specific goal, such as a larger feature or several features, and be validated through Product telemetry (the Product can measure its own usage). Alternatively, it could be for the overall Product, where it is often about the strategic impact and the validation of the efficacy of the implemented strategic deployment [50-54]. Or a combination of both. -->

アウトカムはユーザーの変化を確認する。インパクトは組織の成果を確認する。関連する解釈とともに、将来の適応のための情報として役立ち、理想的には意図したビジネスへの影響を確認することを目的とする。これは、特定の大きな機能や複数の機能などに向けて設定された特定のゴールを対象とし、プロダクトのテレメトリ（プロダクト自身がその利用状況を計測する）によって検証される。あるいは、プロダクト全体を対象とし、戦略的影響や実施された戦略展開[50-54]の有効性の検証に関するものである。またはこれら両方の組み合わせである。

<!-- Favor direct evidence over circumstantial evidence. For example:

- Customer outcomes could Focus on delivering measurable value to customers, such as increased customer satisfaction, customer long-term cost reduction, or the number of customer jobs addressed.
- User outcomes could address specific changes in user behavior that solve problems and improve experiences, like completing tasks more efficiently or engaging with new features.
- Product Stakeholder outcomes could connect these behavioral changes to Product performance metrics, e.g., trends in Product customer, decision-maker/user metrics, Product time to release, time to learn, time to pivot, etc.
- Business impact, e.g., compliance, business long-term cost reduction, business results, trends in market share, customer satisfaction across all Products, organizational time to release, time to learn, time to pivot, etc.
- Scrum Team outcomes such as improved technical capability (psychological flow [70], frequency of release, tooling, skills, technical debt, UX or CX debt, capacity), climate/culture for net improvement and innovation. -->

アウトカム完成の定義は状況証拠よりも直接的な証拠（エビデンス）を優先する。例えば以下のようなものである：

- 顧客のアウトカムは顧客満足度の向上、顧客の長期コスト削減、対応した顧客の案件数など、計測可能な顧客価値の提供に _集中_ することができる
- ユーザーのアウトカムはタスクをより効率的に完了することや新機能の利用など、問題を解決し体験を改善するユーザー行動の具体的な変化に対処することができる
- プロダクトステークホルダーのアウトカムは、これらの行動変化をプロダクトのパフォーマンス指標に結び付けることができる。例えば、顧客、意思決定者/ユーザー指標のトレンド、プロダクトとしてのリリースまでの時間、学習までの時間、ピボットまでの時間など
- ビジネスへの影響。例えば、コンプライアンス、長期的なコスト削減、ビジネス成果、市場シェアの傾向、すべてのプロダクトにわたる顧客満足度、組織としてのリリースまでの時間、学習までの時間、ピボットまでの時間など
- スクラムチームのアウトカム。技術的能力の向上（心理学的フロー状態[46]、リリース頻度、ツール、スキル、技術的負債、UXまたはCX負債、開発能力）、実質的な改善やイノベーションのための風土や文化など

<!-- User eXperience (UX) or Customer eXperience (CX) debt is the sum of design and implementation choices—intentional or not—that make a Product or service less usable, enjoyable, or effective for users or customers. Recognizing, tracking, and addressing this debt is essential for delivering Products that truly meet user needs and expectations. -->

ユーザーエクスペリエンス（UX）負債やカスタマーエクスペリエンス（CX）負債とは、意図的であるか否かに関わらず、プロダクトやサービスをユーザーや顧客にとって使いにくく、楽しめず、効果的でないものとする設計および実装上の選択の総和である。この負債を認識し、追跡し、対処することは、真にユーザーのニーズと期待に応えるプロダクトを提供するために不可欠である。

<!-- Measures over time make Product, market, and Stakeholder trends (including but not limited to customer or user) transparent; these can be reviewed at any time during the Sprint, including the Sprint Review. -->

時間の経過に伴い計測することで、プロダクト、市場、ステークホルダーのトレンド（顧客やユーザーを含むがこれらに限定されない）が透明化される。これらはスプリントレビューを含めスプリントの期間中のいつでも参照可能である。

<!-- ## Increment -->

## インクリメント {#increment}

<!-- The Increment is an artifact. It is the integration of the work completed to the standard of the Definition of Output Done. The Increment is an output and a Product candidate. -->

インクリメントは作成物の一つである。これはアウトプット完成の定義の基準に従って完了した作業を統合したものである。インクリメントはアウトプットでありプロダクトの候補である。

<!-- Multiple Increments may be created within a Sprint through the completion of Product Backlog Items. Each Increment is thoroughly verified, usable, and integrated with all previous Increments. The resulting aggregated Increment is inspected as soon as possible, at the latest at the Sprint Review. The Increment must be usable and useful to enable result feedback. An Increment is central to Scrum as it enables ongoing value validation. -->

プロダクトバックログアイテムの完了により、スプリントでは複数のインクリメントを作成可能である。各インクリメントは徹底的に検証され、利用可能であり、すべての以前のインクリメントと統合されている。結果として得られる集約されたインクリメントは、可能な限り早く、遅くともスプリントレビューで検査される。インクリメントは結果からのフィードバック（結果フィードバック）を可能にするために利用可能かつ有用でなければならない。インクリメントは継続的な価値検証を可能にするため、スクラムの中心的な存在である。

<!-- An Increment-candidate does not qualify as an Increment until it meets the quality standard of the Definition of Output Done. Only an Increment can be released. An Increment should be a concrete stepping stone toward the Product Goal. Increments may be delivered to Stakeholders or released prior to the Sprint Review. _The best value validation is attained through result feedback._ -->

インクリメント候補は、アウトプット完成の定義の品質基準を満たすまでインクリメントとして認められない。リリース可能なのはインクリメントのみである。インクリメントはプロダクトゴールに向けた具体的な踏み⽯となるべきである。スプリントレビューより前にインクリメントをステークホルダーにデリバリーしたり、リリースされたりする可能性がある。_最良の価値検証は結果からのフィードバック（結果フィードバック）を通じて実現される。_

<!-- ## Commitment: Definition of Output Done -->

## コミットメント：アウトプット完成の定義 {#commitment-definition-of-output-done}

<!-- The Definition of Output Done is a commitment. It formally describes the quality measures that express due diligence for the Increment so that it could be delivered to Stakeholders. -->

アウトプット完成の定義はコミットメントの一つである。これはステークホルダーにインクリメントを提供可能とするために適正に評価をしていること（デューデリジェンス）を表す品質基準を正式に記述したものである。

<!-- The Definition of Output Done typically includes (but is not limited to) both technical standards and Product qualities. The Scrum Team creates it if not provided by the organization as a minimum. If there are multiple Scrum Teams on the same Product, they share the same Definition of Output Done as the common foundation but may improve upon it. -->

アウトプット完成の定義は通常、技術的標準とプロダクト品質の両方を含む（ただしこれらに限定されない）。組織から最低限の基準としてアウトプット完成の定義を提供していない場合は、スクラムチームが作成する。プロダクトに関わるスクラムチームが複数ある場合、共通の基盤として同じアウトプット完成の定義を共有するが、それを改善することもできる。

<!-- The Scrum Team is duty-bound to conform to the Definition of Output Done and continuously improve it. The Increment is cumulative. The Definition of Output Done is for the good of the Product and its Stakeholders. The Definition of Output Done is the overall quality standard for the whole Increment, not the specific standard for each item (e.g., Acceptance Criteria). (SGEP more explicit) -->

スクラムチームはアウトプット完成の定義を遵守し、継続的に改善する義務を負う。インクリメントは累積的なものである。アウトプット完成の定義はプロダクトとそのステークホルダーの利益のために存在する。これはインクリメント全体に対する総合的な品質基準であり、個々のアイテムの基準（例：受け入れ基準）ではない（SGEPでより明示的）。

<!-- A released Increment enables result feedback for Definition of Outcome Done value validation. -->

リリースされたインクリメントは、アウトカム完成の定義による価値検証のための結果からのフィードバック（結果フィードバック）を可能にする。

<!-- ## Product Backlog -->

## プロダクトバックログ {#product-backlog}

<!-- The Product Backlog is an artifact. It is the emergent, ordered (sequenced) list of Product Backlog Items needed to attain the Product Goal. The Product Backlog provides Transparency (work clarity) and is the single source of work for the Scrum Team in order to achieve the Product Goal. The Product Owner, always keeping value in mind, guides the ordering of the Product Backlog Items in the Product Backlog. A smaller Product Backlog often provides more Transparency. -->

プロダクトバックログは作成物の一つである。これは創発的かつ順番に並べられた、プロダクトゴールの達成に必要なプロダクトバックログアイテムの一覧である。プロダクトバックログは透明性（作業の明確さ）を提供し、スクラムチームにとってプロダクトゴールを達成するために必要な作業の唯一の情報源である。プロダクトオーナーは常に価値を意識し、プロダクトバックログ内のプロダクトバックログアイテムの順序付けを行う。プロダクトバックログが小さいほど、透明性はより高まる。

<!-- ## Product Backlog Item -->

## プロダクトバックログアイテム {#product-backlog-item}

<!-- A Product Backlog Item is a potentially valuable item in the Product Backlog. It is not necessarily in any specific format. It is intended to deal with a problem or opportunity. It can include Acceptance Criteria that can tell when work is completed, in addition to the Definition of Output Done. One might deliver exactly what was requested but still not deliver sufficient outcomes. So, a Product Backlog Item can also include clearly defined Outcome Criteria that can tell when sufficient value is delivered, in addition to what is already in the Definition of Outcome Done. -->

プロダクトバックログアイテムは、プロダクトバックログ内にある潜在的に価値のあるアイテムである。これは必ずしも特定の形式である必要はない。プロダクトバックログアイテムは問題や機会に対処することを目的としている。アウトプット完成の定義に加えて、作業が完了したことを判断するための受け入れ基準を含むことができる。要求された内容を正確に提供したとしても、十分なアウトカムが得られない場合がある。そのため、アウトカム完成の定義に含まれているものに加えて、十分な価値が提供されたかどうかを示すための明確なアウトカム基準をプロダクトバックログアイテムに含むことができる。

<!-- A Product Backlog Item is a single piece of work that discovers or delivers value. A Product Backlog Item can evolve anytime, even while Product Developers work on it. During refinement, it is broken down into smaller, more understandable (mostly to the Scrum Team) Product Backlog Items that could deliver value. Occasionally, an item in the Product Backlog might not be related to the Product Goal; if this happens often, it's worth examining if the _Focus_ level might not be where it needs to be. The Scrum Team and Stakeholders should _Focus_ on outcomes over outputs, keep the trade-off balance right, and not let the Scrum Team become a 'feature-factory' or 'discovery-factory.' -->

プロダクトバックログアイテムは価値を発見または提供するための単一の作業単位である。プロダクトバックログアイテムは、プロダクト開発者が作業している間であっても、いつでも進化する可能性がある。リファインメントの過程で、価値を提供でき、より小さく、スクラムチームにとってより理解しやすいプロダクトバックログアイテムに分割される。時にはプロダクトバックログ内のアイテムがプロダクトゴールと無関係である場合もある。そのような状況が頻繁に起きるのであれば、_集中_ のレベルが適切に保たれているか検査する価値がある。スクラムチームおよびステークホルダーは、アウトプットよりもアウトカムに _集中_ し、トレードオフのバランスを保ち、スクラムチームが「機能工場」や「発見工場」にならないようにする必要がある。

<!-- ## Acceptance Criteria -->

## 受け入れ基準 {#acceptance-criteria}

<!-- Acceptance Criteria, if they exist, describe when an output for a specific Product Backlog Item is complete, in addition to the Definition of Output Done. Acceptance Criteria in refined items should provide unambiguous clarity on _what_ is requested. Acceptance Criteria include criteria specific to a Product Backlog Item not already addressed in the Definition of Output Done; they can be functional or non-functional. Acceptance Criteria can evolve anytime, even while Product Developers work on them. -->

受け入れ基準が存在する場合、アウトプット完成の定義の記述に加えて、特定のプロダクトバックログアイテムのアウトプットがいつ完了するかを記述する。リファインメントされたアイテムの受け入れ基準は、_何_ が要求されているかについて曖昧さのない明確な基準を示す必要がある。受け入れ基準は、アウトプット完成の定義でまだ扱われていないプロダクトバックログアイテム固有の機能的・非機能的な基準を含む。受け入れ基準は、プロダクト開発者が作業している間であっても、いつでも進化する可能性がある。

<!-- As a subset, outcome criteria, if they exist, describe the intention of the Product Backlog Item; it is the _why_ behind the _what_. The fulfillment of outcome criteria often complements the Definition of Outcome Done for the Product. They can include criteria specific to a Product Backlog Item not already addressed in the Definition of Outcome Done. If questions arise, the outcome criteria provide direction; they can be in the form of a narrative or measures, ideally, the latter. Outcome criteria can evolve anytime, even while Product Developers work on them. -->

アウトカム基準はその一部であり、存在する場合、プロダクトバックログアイテムの意図を記述する。つまり、何（_What_）の背後にあるなぜ（_Why_）を記述するものである。アウトカム基準の達成は、しばしばプロダクトのアウトカム完成の定義を補完する。アウトカム基準は、アウトカム完成の定義でまだ扱われていないプロダクトバックログアイテム固有の基準を含むことがある。疑問が生じた場合、アウトカム基準は方向性を示す。それは、ナラティブ形式または計測可能な指標の形式を取るが、理想的には後者である。アウトカム基準は、プロダクト開発者が作業している間であっても、いつでも進化する可能性がある。

<!-- ## Refinement -->

## リファインメント {#refinement}

<!-- Refinement is an activity. It may be formal (an additional event) (in the SGEP it is a key element) or informal. Refinement is an ongoing emergent process that fosters clarity and reduces risk; it builds enough understanding and confidence that the selected or upcoming Product Backlog Items are ready (can be completed in accordance with the Definition of Output Done within a small number of days, or shorter). Various types of dependencies are considered. -->

リファインメントは活動の一つである。これは正式な場合（追加イベント）（SGEPにおいては重要な要素である）もあれば、非公式な場合もある。リファインメントは明確さを育み、リスクを軽減する継続的な創発プロセスである。これは選択された、または直近で対応予定のプロダクトバックログアイテムが準備完了（アウトプット完成の定義に従って数日以内またはそれより短い時間で完了できる）であるために必要な十分な理解と確信をチームに形成する。様々な種類の依存関係が考慮される。

<!-- Refinement involves breaking down Product Backlog Items into smaller, more understandable (mostly to the Scrum Team) Product Backlog Items. It can add more details such as description, Acceptance Criteria, order, and size. Attributes vary but should be meaningful to the Scrum Team. Refinement can involve research, including but not limited to, problem or opportunity validation, user or customer experience, solution validation. The Product Developers, and nobody else, are responsible for sizing the Product Backlog Items. The Product Owner may influence the Product Developers by helping them understand and select potential trade-offs. -->

リファインメントは、プロダクトバックログアイテムをより小さく、（主にスクラムチームにとって）より理解しやすく分解することを含む。説明、受け入れ基準、並び順、サイズなどの詳細を追加することができる。属性はさまざまあるが、スクラムチームにとって意味のあるものでなければならない。リファインメントには、問題や機会の検証、ユーザーや顧客の体験、ソリューションの検証などの調査活動が含まれるがこれに限定されない。プロダクト開発者のみがプロダクトバックログアイテムのサイズを決定する責任を負う。プロダクトオーナーは、潜在的なトレードオフを理解し、選択できるよう支援することでプロダクト開発者に影響を与えることができる。

<!-- Participants often include Stakeholders and members of the Scrum Team; it is not uncommon for Product Developers to work directly with Stakeholders. Refinement is often supported or facilitated by the Product Owner. The Product Owner can _Focus_ more on Product ownership if the Product Developers have a broad understanding of the Product. Generally speaking, it is a forward-looking activity that offers clarity, direction, and potential _Focus_ for upcoming Sprints. -->

リファインメントの参加者には、多くの場合ステークホルダーやスクラムチームのメンバーが含まれる。プロダクト開発者がステークホルダーと直接作業することも珍しいことではない。リファインメントは、通常プロダクトオーナーにより支援またはファシリテートされる。プロダクト開発者がプロダクトに対する幅広い理解を持っている場合、プロダクトオーナーはプロダクトオーナーシップの発揮により _集中_ できる。一般に、リファインメントは今後のスプリントに向けて明確さ、方向性、潜在的な _集中_ を提供する将来を見据える活動である。

<!-- ## Commitment: Product Goal -->

## コミットメント：プロダクトゴール {#commitment-product-goal}

<!-- The Product Goal is a commitment. It is represented through the Product Backlog, which is owned by the Product Owner. It is the current single, more strategic, ambitious objective (the _why_). It gives direction for the Product and enables _Focus_ for the Product Developers working on the Product. It improves Transparency by providing a clear, valuable direction for the Product Developers to work toward, using a more tactical Sprint Goal (the _why_ for the Sprint). -->

プロダクトゴールはコミットメントの一つである。これはプロダクトオーナーがオーナーであるプロダクトバックログを通じて表現される。プロダクトゴールは現時点における単一かつより戦略的で野心的な目標（なぜ（_Why_））である。プロダクトに方向性を示し、プロダクト開発者がプロダクトに取り組むための _集中_ の源となる。プロダクトゴールはより戦術的な目標であるスプリントゴール（スプリントのなぜ（_Why_））を通じて、プロダクト開発者が向かうべき明確で価値のある方向性を提供し、透明性を高める。

<!-- A Product Goal is the medium-term objective for the Scrum Team and the Stakeholders (and Supporters). The Scrum Team should fulfill (or abandon) one Product Goal before taking on the next. -->

プロダクトゴールはスクラムチームとステークホルダー（およびサポーター）の中期的な目標である。次のプロダクトゴールに移る前に、スクラムチームはひとつのプロダクトゴールを達成（または放棄）しなければならない。

<!-- A Product Goal is usually an as-yet-unproven assertion about value. It can be expressed as one of many things, including a set of hypotheses about closing or lessening satisfaction gaps (outcomes) and their expected business impact. It gets the balance right by focusing on a subset of the multiplicity of Stakeholders' (including but not limited to customers or users) expectations and limits. Through Inspection and Adaptation, it's essential to embrace uncertainty [41], result feedback, side effects, and other learnings. -->

プロダクトゴールは通常、価値に関する未証明の仮説である。満足度ギャップを埋めるもしくは縮小するための仮説（アウトカム）およびそれらがもたらすビジネスへの影響を含む、様々なものひとつとして表現される。それは、多様なステークホルダー（顧客やユーザーを含むがそれに限定されない）の期待や制約の中から、焦点を絞り適切なバランスを取るものである。検査と適応を通じて、不確実性[41]、結果からのフィードバック（結果フィードバック）、副作用、その他の学習を受け入れることが不可欠である。

<!-- ## What about a Product Vision? -->

## プロダクトビジョンについては？ {#what-about-a-product-vision}

<!-- Many organizations work with a Product Vision, which helps visualize a potential future. The Scrum Team can use a Vision as input for considering a Product Goal. A Product Vision is a meaningful, long-term set of valuable desired outcomes. The medium-term Product Goal is often a stepping stone toward a long-term Product Vision. (a thing in SGEP) -->

多くの組織では、未来の可能性を見える化するためにプロダクトビジョンを活用する。スクラムチームは、プロダクトゴールを検討するためのインプットとしてビジョンを用いることができる。プロダクトビジョンは、意味のある長期的な価値のある望ましいアウトカムのまとまりである。中期的なプロダクトゴールは、多くの場合、長期的なプロダクトビジョンに向けた踏み石となる。（SGEPにおける項目）

<!-- As the Scrum Team and Stakeholders inspect and adapt toward the Product Goal, they need to be _open_ to the idea that the Product Vision or Product Goal might also need to adapt. Often, several Product Goals are sequentially achieved while working toward a vision. -->

スクラムチームとステークホルダーがプロダクトゴールに向けての検査と適応を行う際、プロダクトビジョンやプロダクトゴールも適応が必要な場合があるという考えに _公開_ である必要がある。多くの場合、ビジョンに向かって進む中で、複数のプロダクトゴールを一つずつ達成していく。

<!-- The key thing to note is that a Product Vision is often a work of fiction; none of it may be true. Forming hypotheses and running experiments in a direction is essential, and is where Scrum can add the most value. -->

重要な点は、プロダクトビジョンは創作作品であることであり、必ずしも真実とは限らない。仮説を立てて、方向性を持って実験を重ねることが不可欠であり、そこでスクラムが最も価値を発揮する。

<!-- A Product Vision is often inspiring but can be overwhelming. The Product Goal reduces overwhelm by acting as a more tangible vertical slice of a Product Vision or as an enabler for a Product Vision. -->

プロダクトビジョンは多くの場合、刺激的であるが、規模が大きすぎて負担に感じることもある。プロダクトゴールは、プロダクトビジョンのより具体的な垂直スライスや、またはプロダクトビジョン実現のきっかけとなることで、負担感を軽減する。

<!-- ## Sprint Backlog -->

## スプリントバックログ {#sprint-backlog}

<!-- The Sprint Backlog is an artifact. It is composed of the Sprint Goal (the _why_ for the Sprint), the set of Product Backlog Items selected (the _what_, also known as the forecast) for the Sprint, and often has an actionable plan for delivering the Increment (the _how_). It provides Transparency (work clarity) throughout the Sprint. -->

スプリントバックログは作成物の一つである。スプリントゴール（スプリントのなぜ（_Why_））、スプリントのために選んだプロダクトバックログアイテムのセット（何（_What_）をやるのか、つまり予測）、そして、多くの場合、インクリメントを提供するための実行可能な計画（どのように（_How_））で構成される。これにより、スプリント全体を通じた透明性（作業の明確性）が高まる。

<!-- The Sprint Backlog is a plan by and for the Product Developers. It is the Product Developers' viewpoint of the understood work to achieve the Sprint Goal (the why for the Sprint). Suppose a suboptimal scenario where most items in the Sprint Backlog are continually unrelated to the Product Goal. In that case, the _Focus_ and _Commitment_ Scrum Values are not being upheld. -->

スプリントバックログは、プロダクト開発者によるプロダクト開発者のための計画である。これはスプリントゴール（スプリントのなぜ（Why））を達成するために、どんな作業が必要かをプロダクト開発者の視点でまとめている。もしスプリントバックログのほとんどのアイテムがプロダクトゴールと関係ない状況が続いてしまうと、スクラムの _集中_ と _確約_ の価値基準が守られなくなる。

<!-- Within the context of the Sprint Goal, the Product Developers update their plan, even the forecast, throughout the Sprint as more is learned. The Sprint Backlog should have enough work to get started, e.g., start with one or two Product Backlog Items toward the Sprint Goal. (SG2017 idea brought back) The Product Developers inspect their progress toward the Sprint Goal in the Daily Scrum or more often. Product Developers learn to adapt and respond to uncertainty [41]. -->

スプリントゴールの文脈の中においても、プロダクト開発者がより多くのことを学ぶにつれ、スプリント全体を通じた、予測すら含めた計画を更新する。スプリントバックログには、まず始めるのに十分な作業が入っていればよい。例えば、最初は、スプリントゴールに向けた1つまたは2つのプロダクトバックログアイテムで十分だ（SG2017のアイデアを復活）。プロダクト開発者はデイリースクラムにて、またはより頻繁に、スプリントゴールに向けた進捗を検査し、不確実性[41]に適応し対応することを学ぶ。

<!-- ## Commitment: Sprint Goal -->

## コミットメント：スプリントゴール {#commitment-sprint-goal}

<!-- To attain coherence, the Sprint Goal is a commitment created and owned by the Scrum Team (SG2020 Developers owned the commitment). The Sprint Goal is the single unifying objective (coherent with the Product Goal) of the Sprint (the _why_) for the Product Developers, created in Sprint Planning. Delivery of the Sprint Goal is a commitment by the Product Developers. The Sprint Backlog (including the _why_, the _what,_ and, often, the _how_) provides _Focus_ and flexibility regarding the evolving work, thus improving Transparency. -->

一貫性を確保するために、スプリントゴールはスクラムチームによって作成され、所有されるコミットメントの一つである（SG2020では開発者がコミットメントを所有していた）。スプリントゴールはプロダクト開発者にとってのスプリントの唯一のかつ統一された目的（プロダクトゴールと整合している）（なぜ（_Why_））であり、スプリントプランニングで作成される。スプリントゴールの達成はプロダクト開発者による確約である。スプリントバックログ（なぜ（_why_）、なに（_what_）、そして多くの場合どのように（_how_）を含む）は進化する作業に対して _集中_ と柔軟性をもたらし、透明性を向上させる。

<!-- The Sprint Goal encourages the Scrum Team to work together rather than on separate initiatives. If the work turns out to be different from what the Product Developers expected, the Product Developers collaborate with the Product Owner to negotiate possibilities within the Sprint without affecting the Sprint Goal. No one tells the Product Developers how to size or do their work. -->

スプリントゴールはスクラムチームが個別に作業するのではなく、協力して作業することを促進する。もし作業がプロダクト開発者の予想と異なることが判明した場合は、スプリントゴールに影響を与えることがないように、プロダクト開発者はプロダクトオーナーと協力してスプリント内で対応する可能性を調整する。誰もプロダクト開発者に作業の見積りや進め方を指示することはない。

<!-- If there are multiple objectives, as long as they are coherent with the Product Goal it might be ok. Be careful. Consider the trade off of context switching and focus. The Scrum Team should strive to attain balance over time –– balancing current team capabilities and climate, current stakeholder value, potential stakeholder value and time to value. (SGEP considers DevSecOps) -->

複数のゴールがある場合でも、それらがプロダクトゴールと整合性がとれている限りは問題はないかもしれない。ただし、注意が必要だ。コンテキスト切り替えと集中のトレードオフを考慮することである。スクラムチームは、時間をかけてバランスをとるよう努めるべきであり、そのバランスとは現在のチームの能力と風土、現在のステークホルダーへの価値、潜在的なステークホルダーへの価値、そして価値を届けるまでの時間との間で成り立つものである（SGEPではDevSecOpsを考慮している）。

<!-- ## The Scrum Events in the Expansion Pack -->

## 拡張パックにおけるスクラムイベント {#the-scrum-events-in-the-expansion-pack}

<!-- Scrum combines four timeboxed events for Inspection and Adaptation within a containing fifth event of determinate consistent length, the Sprint. These events support the Scrum pillars of Transparency, Inspection, and Adaptation. Releases enable value, ideally, continuously. Infrequent releases lead to delayed result feedback. -->

スクラムでは検査と適応のための4つのタイムボックス化されたイベントを組み合わせている。それらを包含するイベントは「スプリント」と呼ばれ、決められた一貫した長さのスクラムの5つ目のイベントである。これらのイベントはスクラムの三本柱「透明性」「検査」「適応」を支える。リリースは理想的には継続的な価値の創出を可能にする。頻度の少ないリリースは、結果からのフィードバック（結果フィードバック）の遅延を招く。

<!-- A timebox is a stipulated maximum amount of elapsed time from beginning to end for a defined event, not to be confused with an expectation to use that full amount of time. The purpose of a timebox in Scrum is to foster the selection of essential work, creating _Focus_ to achieve desired results quickly. -->

タイムボックスとは、スクラムで定義されているイベントの開始から終了までの経過時間の上限を規定したものである。そのすべての時間を使い切ることを期待したものではない。スクラムにおけるタイムボックスの目的は、そのイベントの本質的な作業に絞ることを促し、望ましい成果を迅速に達成するための _集中_ を生み出すことである。

<!-- Events create cadence and minimize the need for other meetings not part of Scrum. Ideally, each event is held at the same time and place to reduce complexity [12-17] and foster the formation of habits. Skilled facilitation improves effectiveness. Ineffective events risk losing emphasis on the Sprint Goal, Product Goal, Transparency, Inspection, Adaptation, and Scrum Values. -->

イベントはケイデンスを作り出し、スクラムに含まれない他の会議の必要性を最小限に抑える。理想的には、各イベントは同じ時間・場所で開催されることで、複雑性[12-17]を軽減し、習慣の形成を促す。熟練したファシリテーションは効果性を高める。効果性の低いイベントは、スプリントゴール・プロダクトゴール・透明性・検査・適応・スクラムの価値基準に重点を置かなくなるリスクがある。

<!-- Each event has its own purpose and should include deep, meaningful work. Together, the Scrum events provide a scaffold of Transparency to inspect and adapt, pause, and reflect. The Scrum events support structured thinking and working, effectiveness, and a balanced workload. (SGEP is influenced by Cynefin and Evidence-Based Management) -->

スクラムの各イベントにはそれぞれの目的があり、深く意味のある作業を含むべきである。スクラムイベントは、検査と適応、立ち止まり、振り返りのための土台となる透明性を提供する。これらのイベントは、構造化された思考と作業、効果性、そしてバランスの取れた作業負荷を支える（SGEPはクネビンフレームワークとエビデンスベースドマネジメントの影響を受けている）。

<!-- Communication is key to ensuring the Scrum Team and Supporters _Focus_ on the right thing. Apart from the Sprint, events may consume less time as long as coherence is not lost. -->

スクラムチームおよびサポーターが適切な対象に _集中_ するためには、コミュニケーションが鍵となる。スプリント以外のイベントは、一貫性が損なわれない限り、より短い時間で行うことも可能である。

<!-- ## The Sprint -->

## スプリント {#the-sprint}

<!-- The Sprint is an event where ideas are turned into value. The Sprint is the container event. It is an iteration of a determinate time in which work is carried out. It provides _Focus_ and stability. A Sprint is no longer than four weeks. A new Sprint starts immediately after the conclusion of the previous Sprint. All the work necessary to achieve the Product Goal happens within Sprints. -->

スプリントはイベントの一つであり、ここでアイデアが価値に変わる。スプリントは入れ物となるイベントである。作業が実施される定められた期間の反復である。スプリントは _集中_ と安定性をもたらす。スプリントは最大で4週間である。前のスプリントの終了直後に新しいスプリントが始まる。プロダクトゴールを達成するために必要なすべての作業はスプリント内で行われる。

<!-- Sprints are the heartbeat of Scrum, where the Scrum Team turns ideas into usable, useful, and potentially valuable Increments. The Increment is released as soon as practically possible, considering the need for early result feedback. A lack of release to some subset of Stakeholders (including but not limited to real customers, decision-makers, and users) can lead to a lack of timely result feedback. Multiple Increments may be created in a Sprint; the Scrum Team should strive to validate value through early and frequent releases, where applicable. -->

スプリントはスクラムにおける心臓の鼓動であり、スクラムチームがアイデアを利用可能で、有用で、潜在的に価値のあるインクリメントへと変える場である。インクリメントは早期の結果からのフィードバック（結果フィードバック）の必要性を考慮し、可能な限り早くリリースされる。一部のステークホルダー（顧客、意思決定者、ユーザーを含むがこれらに限定されない）へリリースがされていないと、タイムリーに結果からのフィードバック（結果フィードバック）が得られなくなる。スプリントでは複数のインクリメントが作成されることもある。スクラムチームは可能な限り早期かつ頻繁にリリースし価値検証を行うよう努めるべきである。

<!-- During the Sprint:

- No changes are made that would endanger the Sprint Goal;
- The Increment(s) should not decrease in quality;
- The Product Backlog is refined as needed; and,
- As more is learned, current work may be clarified and renegotiated with the Product Owner without affecting the Sprint Goal. -->

スプリントでは、

- スプリントゴールの達成を危険にさらすような変更はしない。
- インクリメントにより品質を低下させるべきではない。
- プロダクトバックログを必要に応じてリファインメントする。
- より多くの知見を得るにつれて、現在の作業は明確化され、スプリントゴールに影響を与えない範囲でプロダクトオーナーと再交渉される可能性がある。

<!-- Sprints enable outcomes by ensuring Inspection and Adaptation of progress toward a Sprint Goal at least every four weeks. When a Sprint is too long, the Sprint Goal may become incoherent, increasing complexity [12-17] and risk. Shorter Sprints often generate more learning cycles; they could also limit risk. -->

スプリントによって、スプリントゴールに対する進捗の検査と適応を少なくとも4週間ごとに確実に行うことで、アウトカムが実現される。スプリントが長すぎると、スプリントゴールが一貫性を失い、複雑性[12-17]とリスクが増加する。スプリントの期間を短くすれば、より多くの学習サイクルを作り出す可能性があり、同時にリスクを軽減できる。

<!-- Shorter Sprints usually require improved capabilities (e.g., refining, vertical slicing, technical domain, business domain). Context matters and the Scrum Team strives to strike the right balance. -->

スプリントを短くするには、リファインメント、垂直スライス、技術ドメインおよびビジネスドメインの知識といった能力の向上が求められる。文脈は重要であり、スクラムチームは適切なバランスを取るよう努める。

<!-- Various complementary practices exist to assess or forecast progress, like burn-downs, burn-ups, flow analytics, Monte Carlo probabilistic forecasts, large effort estimation, fuzzy sets [55], etc. While useful, these do not replace the importance of empiricism [19]. In complex [12-17] environments, what has already happened may be used for forward-looking decision-making, but what will happen is unknown. -->

進捗の評価や予測のための様々な補完的なプラクティスが存在する。例えば、バーンダウン、バーンアップ、フロー分析、モンテカルロ法、大規模工数見積もり、ファジィ集合[55]などである。これらは有用であるが、経験主義[19]の重要性を置き換えるものではない。複雑な[12-17]環境下では、すでに発生したことは将来を見据えた意思決定に使用されるが、これから何が起きるかはわからない。

<!-- You could think about a Sprint as a mini project with a clear outcome, determinate length and understood costs. However, the various work activities happen in parallel and not in a sequential defined linear way. -->

スプリントは、明確な成果、定められた期間、明確なコストを持つミニプロジェクトと考えることもできる。ただし、さまざまな作業は並行して発生し、順序が定められた線形的な方法では実行されない。

<!-- A Sprint could be canceled if the Sprint Goal becomes obsolete. Only the Product Owner has the authority to cancel the Sprint. Shorter Sprints lower the likelihood of a cancellation. -->

スプリントゴールがもはや役に立たなくなった場合、スプリントは中止されることになるだろう。プロダクトオーナーだけがスプリントを中止する権限を持つ。スプリントが短いほど、中止の可能性は低くなる。

<!-- ## Sprint Planning -->

## スプリントプランニング {#sprint-planning}

<!-- Sprint Planning is an event. This first event of the Sprint is where the Scrum Team gives _Focus_ and creates commitment. -->

スプリントプランニングはイベントの一つである。スプリントの最初のイベントであり、スクラムチームが _集中_ を高め、コミットメントを生み出す場である。

<!-- During Sprint Planning, the more strategic Product Goal (the _why_ for the Product Backlog) is considered and provides direction. In doing so, the Product Developers create the Sprint Backlog, which consists of the short-term, more tactical Sprint Goal (the _why_ for the Sprint), the initially identified work, and the plan to deliver. -->

スプリントプランニングにおいて、より戦略的なプロダクトゴール（プロダクトバックログにおけるなぜ（_Why_））が考慮され、方向性が提供される。スプリントプランニングの過程で、プロダクト開発者はスプリントバックログを作成する。スプリントバックログには短期的かつより戦術的なスプリントゴール（スプリントにおけるなぜ（_Why_））、最初に特定された作業、そしてデリバリーのための計画が含まれる。

<!-- Sprint Planning addresses the following topics: -->

スプリントプランニングは次のトピックに対応する：

<!-- ## The _Why_ for the Sprint -->

## スプリントのなぜ（_Why_） {#the-why-for-the-sprint}

<!-- The Product Owner proposes data-informed ideas (e.g., Refinement, result feedback, other learnings) for how the Product could increase its value and utility in the current Sprint. The Product Owner and the Product Developer collaborate to define a Sprint Goal that communicates why the Sprint is valuable to Stakeholders toward the Product Goal (SGEP emphasizes directional, just-in-time planning). The Sprint Goal must be finalized by the end of Sprint Planning. -->

プロダクトオーナーは、プロダクトの価値と有用性を今回のスプリントでどのように高めることができるかについて、データに基づくアイデア（例：リファインメント、結果からのフィードバック、その他の学び）を提案する。プロダクトオーナーとプロダクト開発者が協力して、プロダクトゴールに向けてそのスプリントにはなぜ価値があるかをステークホルダーに伝えるスプリントゴールを定義する（SGEPは方向性のある、ジャストインタイム計画を強調している）。スプリントゴールは、スプリントプランニングの終了までに確定する必要がある。

<!-- ## The _What_ toward the _Why_ -->

## なぜ（_Why_）に向けた何（_What_） {#the-what-toward-the-why}

<!-- Through collaboration with the Product Owner, the Product Developers select items from the Product Backlog to include in the current Sprint. The Scrum Team may refine these items, which increases understanding and confidence. Selected items should be achievable according to the standard of the Definition of Output Done, alongside other items. -->

プロダクト開発者は、プロダクトオーナーとの協働を通して、プロダクトバックログからアイテムを選択し、今回のスプリントに含める。スクラムチームはプロダクトバックログアイテムのリファインメントをする場合がある。それによって、チームの理解と自信が高まる。選択されたプロダクトバックログアイテムは、他のアイテムと同様にアウトプット完成の定義の基準に従って達成可能である必要がある。

<!-- Selecting how much can be completed within a Sprint may be challenging. However, the more the Product Developers know about their past performance, vertical slicing, upcoming capacity, and the Definition of Output Done, the more confident they will be in their ability to forecast Sprint outcomes. -->

スプリント内でどれくらい完了できるかを選択するのは難しいかもしれない。しかしながら、プロダクト開発者が過去の自分たちのパフォーマンス・垂直スライス・今回のキャパシティ・アウトプット完成の定義の理解を深めていけば、スプリントのアウトカムを予測する能力に自信が持てるようになる。

<!-- Successful Scrum Teams do not overload themselves. In fact, they plan to finish work early, sometimes using a buffer for unexpected events [56]. This helps the Scrum Team to stay focused, improve quality, and satisfy Stakeholders by delivering value sooner. Chronic overload or sudden shifts can cause excessive negative stress, which Jeff Sutherland calls 'Bayesian surprise.' They can disrupt the Scrum Team's psychological flow [46] and performance. Clear communication, professional handling of emergence [21], and small, regular changes help prevent this, so Scrum Teams should aim for early delivery. (SGEP supports slack) -->

成功するスクラムチームは過剰な負荷をかけない。実際、成功するスクラムチームは作業を早めに完了できるよう計画し、予期せぬ事態に備えてバッファを設けることもある[56]。これによりスクラムチームは集中を維持し、品質を向上させ、より早く価値をデリバリーすることでステークホルダーを満足させることができる。慢性的な過負荷や突然の変化は、Jeff Sutherlandが「ベイジアン・サプライズ」と呼ぶ過度なストレスを引き起こし、スクラムチームの心理学的フロー[46]やパフォーマンスに悪影響を及ぼす。明確なコミュニケーション、創発へのプロフェッショナルな対応[21]、そして小さな変化を日常的に行うことで、こうした事態を防ぐ事ができる。このような理由から、スクラムチームは早期のデリバリーを目指すべきである（SGEPはスラックを支持している）。

<!-- ## The _How_ for the _What_ -->

## 何（_What_）に対するどのように（_How_） {#the-how-for-the-what}

<!-- How the work is done is at the sole discretion of the Product Developers. No one else tells the Product Developers how to do their work. The Product Developers select their own work; no one else assigns or pushes Product Backlog Items to the Product Developers, not even the Product Owner. -->

作業の進め方はプロダクト開発者の裁量に委ねられている。他の誰もプロダクト開発者に作業の方法を指示することはできない。プロダクト開発者は自ら作業を選択する。プロダクトバックログアイテムをプロダクト開発者に割り当てたり押し付けたりすることは他の誰にもできない。プロダクトオーナーであっても、それは同様である。

<!-- Sprint Planning is timeboxed to a maximum of eight hours for a four-week Sprint. The event is usually shorter for shorter Sprints. Context matters. But as a rule of thumb, do enough planning to get started with the work, e.g., plan a few Product Backlog Items toward the Sprint Goal. -->

スプリントが4週間の場合、スプリントプランニングのタイムボックスは最大で8時間である。スプリントの期間が短ければスプリントプランニングの時間も短くすることが多い。文脈は重要である。しかし、経験則として、作業を開始できるだけの計画、例えばスプリントゴールに向けていくつかのプロダクトバックログアイテムを計画するだけでもよい。

<!-- ## Daily Scrum -->

## デイリースクラム {#daily-scrum}

<!-- The Daily Scrum is an event. At the Daily Scrum, the Product Developers collaborate on progress toward the Sprint Goal and update the actionable plan, the Sprint Backlog, until the next Daily Scrum. In the event the Sprint Goal has already been achieved, the Product Developers collaborate on meaningful progress toward the Product Goal. (SGEP emphasizes direction) -->

デイリースクラムはイベントの一つである。デイリースクラムにおいて、プロダクト開発者はスプリントゴールに向けた進捗について協働し、次のデイリースクラムまで実行可能な計画であるスプリントバックログを更新する。スプリントゴールがすでに達成されている場合、プロダクト開発者はプロダクトゴールに向けた意味のある進捗について協働する（SGEPは方向性を強調している）。

<!-- The Daily Scrum provides _Focus_, cohesion, and urgency and fosters self-management [11]. Usually, only the Product Developers participate. To simplify, it often uses the same meeting cadence, place, and time. -->

デイリースクラムは、_集中_、一体感、緊迫感をもたらし、自己管理を促進する[11]。通常、参加するのはプロダクト開発者のみである。簡素化のため、同じ会議のケイデンス、場所、時間を採用することが多い。

<!-- The Product Developers can select whatever structure and techniques they want. Daily Scrums improve communication towards attaining the Sprint Goal, identify and address risks and impediments, promote quick decision-making, and consequently eliminate the need for other meetings. -->

プロダクト開発者は、任意の構造ややり方を選択できる。デイリースクラムは、スプリントゴールの達成に向けたコミュニケーションを改善し、リスクや障害の特定と対処を行い、迅速な意思決定を促進する。その結果、他の会議を不要にする。

<!-- The Daily Scrum is not the only time the Product Developers adjust their plan for the Sprint within the context of the Sprint Goal or Product Goal. Product Developers often meet throughout the day for more detailed discussions. -->

プロダクト開発者がスプリントゴールやプロダクトゴールの文脈においてスプリントの計画を調整するのは、デイリースクラムのときだけではない。プロダクト開発者は、より詳細な議論をするために、一日を通じて頻繁に話し合う。

<!-- To enable the flow of value [48-49] and enable potential outcomes sooner, the Product Developers should focus on one item or a few items at a time and meet the Definition of Output Done, before starting to work on other items. The Product Developers can achieve this by focusing, having fewer items in progress, and proactively finishing work over starting new work. The Product Developers monitor idle work, not idle people. (SGEP emphasizes flow) -->

価値のフロー[48-49]を促進し、潜在的なアウトカムをより早く実現するために、プロダクト開発者は一度に1つまたは少数のアイテムに集中し、他のアイテムの作業を開始する前にアウトプット完成の定義を満たすべきである。プロダクト開発者は、集中し、進行中のアイテムを少なくし、新しい作業を開始するよりも能動的に作業を完了することで、これを達成することができる。プロダクト開発者が監視するのは、稼働していない人ではなく、停滞している作業である（SGEPはフローを強調している）。

<!-- The Daily Scrum is timeboxed to fifteen minutes per day. -->

デイリースクラムは1日あたり15分間のタイムボックスである。

<!-- ## Sprint Review -->

## スプリントレビュー {#sprint-review}

<!-- The Sprint Review is an event. It is an interactive, collaborative working session. Often, the Scrum Team shares the current Product Goal and presents the Definition of Output Done and the Definition of Outcome Done to the Stakeholders. The Scrum Team shares the results of their work, what trade-offs were made, and how much progress was made toward the Product Goal (the why behind the work). If available, current and up-to-date measures of progress toward the Definition of Outcome Done are shared and considered. -->

スプリントレビューはイベントの一つである。これは相互作用があり協働的なワーキングセッションである。通常、スクラムチームは現在のプロダクトゴールを共有し、アウトプット完成の定義とアウトカム完成の定義をステークホルダーに提示する。スクラムチームは作業の結果、どのようなトレードオフが行われたか、プロダクトゴールに向けてどれだけの進捗が行われたか（作業の背後にあるなぜ）を共有する。可能であれば、アウトカム完成の定義に向けた進捗の現時点かつ最新の指標が共有され検討される。

<!-- The Sprint Review inspects many things related to the Product, such as the Product Goal, Product Backlog, the Sprint Goal, the learnings, the Increment, Stakeholder expectations and limits, result feedback, side effects, progress with the Product, the market, as well as forward-looking, e.g., what new ideas and opportunities have emerged, potential next steps. -->

スプリントレビューは、プロダクトゴール、プロダクトバックログ、スプリントゴール、学び、インクリメント、ステークホルダーの期待と制約、結果からのフィードバック（結果フィードバック）、副次的な影響、プロダクトの進捗状況、市場動向、さらに、将来を見据えた事項——新たに生まれたアイデアや機会、次に取り得る可能性のあるステップなど——について検査する。

<!-- Informed by what is learned:

- Participants sense, listen, learn, and collaborate on what to potentially do next;
- The Product Backlog (the what) is adapted and possibly the Product Goal, ideally supported by evidence or observations and guided by the Product Goal or optional Product Vision; and,
- Participants adapt the Product's Definition of Outcome Done for future Sprints. -->

学習したことに基づいて：

- 参加者は次に潜在的に何をすべきかについて感知し、傾聴し、学び、協働する
- プロダクトバックログ（何）が適応され、場合によってはプロダクトゴールも、理想的にはエビデンスや観察結果に裏打ちされ、プロダクトゴールまたは任意のプロダクトビジョンによって方向づけられる
- 参加者は将来のスプリントのためにプロダクトのアウトカム完成の定義を適応させる

<!-- It's always important to consider Stakeholders and what they value, including inanimate, non-human Stakeholders such as the law. -->

ステークホルダーと彼らが価値を置くものを考慮することは常に重要である。ステークホルダーには、法律といった、生物でも人間でもないものも含まれる。

<!-- Incomplete Product Backlog Items return to the Product Backlog for future consideration and are not presented; sometimes, they are moved into the next Sprint. -->

未完了のプロダクトバックログアイテムは将来の検討のためにプロダクトバックログに戻され、提示されない。場合によっては、次のスプリントに移されることもある。

<!-- The Sprint Review is the second-to-last event of the Sprint and is timeboxed to four hours for a four-week Sprint. For shorter Sprints, the event is usually shorter. -->

スプリントレビューは、スプリントの最後から2番目のイベントであり、スプリントが4週間の場合、タイムボックスは最大4時間である。スプリントの期間が短ければ、スプリントレビューの時間も短くすることが多い。

<!-- ## Sprint Retrospective -->

## スプリントレトロスペクティブ {#sprint-retrospective}

<!-- The Sprint Retrospective is an event. At this event, the Scrum Team agrees on how to improve. Bad assumptions are also explored, i.e., assumptions that led the Scrum Team in the wrong direction. Good things like particular technologies, processes, patterns, etc., might also be pointed out or reinforced. Inspected elements often vary with the domain of work. Reflection is more effective in a psychologically safe environment. -->

スプリントレトロスペクティブはイベントの一つである。このイベントにおいて、スクラムチームは改善方法について合意する。誤った仮説、すなわちスクラムチームを誤った方向に導く仮説についても検討される。また、有益な事項——特定の技術、プロセス、パターンなど——が指摘されたり、強調されたりすることもある。検査される要素は、作業領域によってしばしば異なる。振り返りは、心理的安全性のある環境においてこそ、より効果的に行われる。

<!-- The Sprint Retrospective focuses on the most helpful changes to improve, such as:

- The Increment
- Outcomes and business impact
- Professionalism, e.g., skills, technical practices, tooling, ability to innovate;
- Flow of validated value [48-49], e.g., end-to-end flow metrics, time-to-market;
- Effectiveness (the _how_), e.g., technology, processes, dependencies;
- Interactions and Scrum Team dynamics, e.g., collaboration, working arrangements;
- Information radiators, e.g., product wall, metrics;
- The Definition of Output Done for future Sprints;
- Further adaptations to the Definition of Outcome Done for future Sprints;
- How to automatically attain the measures regarding the Definition of Outcome Done;
- And more. -->

スプリントレトロスペクティブは以下のような改善に最も役立つ変更に焦点を当てる：

- インクリメント
- アウトカムとビジネスへの影響
- プロフェッショナリズム。例：スキル、技術的実践、ツール活用、イノベーションの能力
- 検証済み価値のフロー[48-49]。例：エンドツーエンドフロー指標、市場に出すまでの時間
- 効果性（_どのように_）。例：技術、プロセス、依存関係
- 相互作用とスクラムチームダイナミクス。例：協働、ワーキングアグリーメント
- 情報ラジエーター。例：プロダクトウォール、各種指標
- 将来のスプリントのためのアウトプット完成の定義
- 将来のスプリントのためのアウトカム完成の定義へのさらなる適応
- アウトカム完成の定義に関する指標の自動取得方法
- その他

<!-- The most impactful improvements should be addressed as soon as possible. The Scrum Team should not just talk about improvement; Scrum depends on meaningful, continuous improvement follow-through. Some improvement actions rely on the assistance of Supporters, but that does not mean the Scrum Team should not strive for net improvement regardless (such as continual marginal gains). -->

最も影響の大きな改善は、できるだけ早く対処する。スクラムチームは単なる改善の議論に終始すべきではない。スクラムは意味のある継続的改善の徹底に依存する。いくつかの改善アクションはサポーターの支援に依存するが、それはスクラムチームが改善に向けた純粋な前進、たとえば継続的なわずかな成果の積み重ねを目指すべきでないということを意味するものではない。

<!-- The Sprint Retrospective concludes the Sprint. It is timeboxed to three hours for a four-week Sprint. For shorter Sprints, the event is usually shorter. -->

スプリントレトロスペクティブをもってスプリントは終了する。スプリントが4週間の場合、スプリントレトロスペクティブは最大3時間である。スプリントの期間が短ければ、スプリントレトロスペクティブの時間も短くすることが多い。

<!-- ## End Note -->

## 最後に {#end-note}

<!-- Scrum is like a mirror. If the image in the mirror is not as expected, should the mirror be hidden? -->

スクラムは鏡のようなものである。鏡に映る像が期待通りでない場合、その鏡を隠すべきであろうか？

<!-- Attain at least one Increment each Sprint as a habit before you adapt Scrum. Every part of Scrum has a purpose; understanding the why for each part is essential. Consider the context. The short-term is about delivery. The long-term is about successful emergent change in a direction and the sustainable delivery of value: outcomes for Stakeholders and impact for organizations. Successful Scrum adoption depends on getting the balance right between the short and long terms. -->

スクラムを適用する前に、スプリント毎に少なくとも1つのインクリメントを作成することを習慣化する。スクラムのすべての部分には目的がある。各部分の「なぜ」を理解することが不可欠である。文脈を考慮すること。短期的にはデリバリーが重要である。長期的には望ましい方向への創発的な変化の成功と持続可能な価値の提供——ステークホルダーにとってのアウトカムと組織にとってのインパクト——が重要である。スクラム適用の成功は、短期と長期のバランスを適切に取ることにかかっている。

<!-- Be careful about copying approaches from other organizations without also fostering their culture. Emergent change in the direction of travel is the change. The change includes (but is not limited to) leadership, workflows, processes, and systems, including HR, Finance, Procurement, and more. Scrum is part of a never-ending expedition of continual improvement and evolution in a direction of travel rather than a destination. -->

他の組織からアプローチを模倣する際には、その組織の文化を育むことなしにアプローチを模倣することは慎重にすべきである。望ましい方向への創発的な変化こそが変化である。その変化にはリーダーシップ、ワークフロー、プロセス、人事、財務、調達などのシステムが含まれるが、これらに限定されない。スクラムは目的地ではなく、望ましい方向に向けた継続的改善と進化の終わりなき旅の一部である。

<!-- ## Acknowledgments -->

## 謝辞 {#acknowledgments}

<!-- Scrum was inspired by Lean [20], the Toyota Production System [57-58], the Harvard Business Review article 'The New New Product Development Game' by Hirotaka Takeuchi and Ikujiro Nonaka [18], and Empiricism at Dupont [59]. -->

スクラムは、リーン[20]、トヨタ生産方式[57-58]、竹内弘高と野中郁次郎によるハーバード・ビジネス・レビューの記事「The New New Product Development Game」[18]、デュポン社における経験主義[59]から着想を得ている。

<!-- Scrum was developed in the early 1990s. Ken Schwaber and Jeff Sutherland first co-presented Scrum at the OOPSLA Conference in 1995 [60]. The first version of the [Scrum Guide](https://scrumguides.org/) [7] appeared in 2009. Scrum is evolving. -->

スクラムは1990年代初頭に開発された。Ken SchwaberとJeff Sutherlandは1995年のOOPSLAカンファレンスにて初めてスクラムを共同発表した[60]。[スクラムガイド](https://scrumguides.org/)[7]の初版は2009年に公開された。スクラムは進化を続けている。

<!-- We also thank reviewers who provided feedback to earlier drafts, including but not limited to, Daryn Basson, Alex Benes, Kurt Bittner, Deb Bhattacharya, Magdalena Firlit, Nichervan Fazel, Peter Fischbach, Michael Forni, Tom Gilb, Martin Hinshelwood, Jesse Houwing, Michael Huynh, Matthew Ijogi, Marc Kaufmann, Tom Mellor, Christian Neverdal, Stas Pavlov, Ian Sharp, Alisa Stolze, Mark Summers, and Nader Talai. -->

初期草稿にフィードバックを提供した以下を含むがこれらに限定されない、レビュアーに感謝する。Daryn Basson, Alex Benes, Kurt Bittner, Deb Bhattacharya, Magdalena Firlit, Nichervan Fazel, Peter Fischbach, Michael Forni, Tom Gilb, Martin Hinshelwood, Jesse Houwing, Michael Huynh, Matthew Ijogi, Marc Kaufmann, Tom Mellor, Christian Neverdal, Stas Pavlov, Ian Sharp, Alisa Stolze, Mark Summers, and Nader Talai

<!-- ## Attribution for the Scrum Guide Expansion Pack Collection -->

## スクラムガイド拡張パックコレクションの帰属 {#attribution-for-the-scrum-guide-expansion-pack-collection}

<!-- This collection was written and compiled by _Ralph Jocham, John Coleman, and Jeff Sutherland_. Each section is individually attributed above and retains its original license. The collection as a whole is for informational purposes; please respect the license terms of each section. -->

本コレクションは _Ralph Jocham、John Coleman、Jeff Sutherland_ によって執筆・編集された。各セクションは上記に個別に帰属が記載されており、元のライセンスを保持している。コレクション全体は情報提供を目的としている。各セクションのライセンス条項を尊重されたい。

<!-- ## References -->

## 参考文献 {#references}

\[1\] Langton, C.G. (ed.) (1989) Artificial Life: Proceedings of an Interdisciplinary Workshop on the Synthesis and Simulation of Living Systems, Los Alamos, New Mexico, September 1987\. Santa Fe Institute Studies in the Sciences of Complexity, vol. VI. Redwood City, CA: Addison-Wesley.
\[2\] Langton, C.G. (1989) 'Life at the edge of chaos', in Langton, C.G. (ed.) Artificial Life: Proceedings of an Interdisciplinary Workshop on the Synthesis and Simulation of Living Systems. Santa Fe Institute Studies in the Sciences of Complexity, vol. VI. Redwood City, CA: Addison-Wesley, pp. 41–91.
\[3\] Holland, J.H. (1992) Complex Adaptive Systems. Daedalus, 121(1), pp. 17–30. Available at: [https://www.jstor.org/stable/20025416](https://www.jstor.org/stable/20025416) (Accessed: 17 May 2025).
\[4\] Axelrod, R. and Cohen, M.D. (2000) Harnessing Complexity: Organizational Implications of a Scientific Frontier. New York: Free Press.
\[5\] Juarrero, A. (1999) Dynamics in Action: Intentional Behavior as a Complex System. Cambridge, MA: MIT Press.
\[6\] Snowden, D.J. and Boone, M.E. (2007) 'A leader's framework for decision making'（日本語訳版: 「クネビンフレームワーク」による臨機応変の意思決定手法）, Harvard Business Review, 85(11), pp. 68–76. Available at: [https://hbr.org/2007/11/a-leaders-framework-for-decision-making](https://hbr.org/2007/11/a-leaders-framework-for-decision-making) (Accessed: 17 May 2025\)
\[7\] Schwaber, K. & Sutherland, J. (2020) The Scrum Guide: The definitive guide to Scrum: The rules of the game（日本語訳版: スクラムガイド）. Available at: [https://scrumguides.org/docs/scrumguide/v2020/2020-Scrum-Guide-US.pdf](https://scrumguides.org/docs/scrumguide/v2020/2020-Scrum-Guide-US.pdf) (Accessed: 17 May 2025\)
\[8\] Schwaber, K. (2023) 'Scrum Guide', Ken Schwaber's Blog, 25 September. Available at: [https://kenschwaber.wordpress.com/2023/09/25/scrum-guide/](https://kenschwaber.wordpress.com/2023/09/25/scrum-guide/) (Accessed: 20 May 2025).
\[9\] Mayer, T. (2025) A Simple Guide to Scrum. \[Online\]. Available at: [https://scrum.academy/guide/](https://scrum.academy/guide/) (Accessed: 17 May 2025\)
\[10\] Scrum.org (2025) Scrum Hexis. Available at: [https://thecynefin.co/product/hexi-scrumorg/?srsltid=AfmBOorcohLYeVy0qBsQFI6mK_bZtJA_uGC6hPL2BdptiTwNmMwpKTQv](https://thecynefin.co/product/hexi-scrumorg/?srsltid=AfmBOorcohLYeVy0qBsQFI6mK_bZtJA_uGC6hPL2BdptiTwNmMwpKTQv) (Accessed: 17 May 2025).
\[11\] LeSS.works (n.d.) Self-managing teams. Available at: [https://less.works/less/management/self-managing-teams](https://less.works/less/management/self-managing-teams) (Accessed: 17 May 2025).
\[12\] [Cynefin.io](https://Cynefin.io/), V. (2022) Cynefin wiki, [Cynefin.io](https://Cynefin.io/). [Cynefin.io](https://Cynefin.io/). At: [https://cynefin.io/](https://cynefin.io/) (Accessed: April 4, 2023).
\[13\] Rancati, A. and Snowden, D. (2021) Managing complexity (and chaos) in a crisis \- a field guide for decision makers inspired by the Cynefin framework. Luxembourg, Belgium: Publications Office of the European Union.
\[14\] Snowden, D. et al. (2022) Cynefin® weaving sense-making into the fabric of our world. 2nd edn. Edited by R. Greenberg and B. Bertsch. Singapore, Singapore: Cognitive Edge \- The Cynefin Co.
\[15\] Snowden, D. (2023) Cynefin St David's 2023 1 of 2, Cynefin Co. [https://thecynefin.co/cynefin-st-davids-2023-1-of-2/](https://thecynefin.co/cynefin-st-davids-2023-1-of-2/) (Accessed: April 20, 2023).
\[16\] Snowden, D. (2023) Managing for emergence through abduction, The Cynefin Co. At: [https://thecynefin.co/managing-for-emergence/](https://thecynefin.co/managing-for-emergence/) (Accessed: June 24, 2023).
\[17\] Snowden, D. and Smith, N. (2023) Leadership discussion: Dave and Natalie \- the Cynefin co, YouTube. At: [https://youtu.be/WcPZ8ybDF0w](https://youtu.be/WcPZ8ybDF0w) (Accessed: April 7, 2023).
\[18\] Takeuchi, H. and Nonaka, I. (2014) The new new product development game（日本語訳版: 新たなる新製品開発の方法）, Harvard Business Review. At: [https://hbr.org/1986/01/the-new-new-product-development-game](https://hbr.org/1986/01/the-new-new-product-development-game) (Accessed: 21 January 2024).
\[19\] Campbell, J. (2025) 'Empiricism', EBSCO Research Starters. Available at: [https://www.ebsco.com/research-starters/religion-and-philosophy/empiricism](https://www.ebsco.com/research-starters/religion-and-philosophy/empiricism) (Accessed: 17 May 2025\)
\[20\] Womack, J.P. and Jones, D.T. (1996) Lean Thinking: Banish Waste and Create Wealth in Your Corporation（日本語訳版: リーン・シンキング）. New York: Simon & Schuster.
\[21\] Templeton Foundation (2023) 'What Is Emergence?' John Templeton Foundation. Available at: [https://www.templeton.org/news/what-is-emergence](https://www.templeton.org/news/what-is-emergence) (Accessed: 17 May 2025).
\[22\] Wolfram, S. (2002) A new kind of science. Champaign, IL: Wolfram Media.
\[23\] Sutherland, J., Coplien, J.O., Heasman, L., den Hollander, M., Ramos, C. and The Scrum Patterns Group (2019) A Scrum Book: The Spirit of the Game. Raleigh, NC: Pragmatic Press.
\[24\] Alexander, C. (1979) The timeless way of building（日本語訳版: 時を超えた建設の道）. New York: Oxford University Press.
\[25\] Lewis, R. (2023) An operating model for business agility: Agile for managers of the digital age. Independently published.
\[26\] less.works (n.d.) Technical Excellence（日本語訳: 技術的長所）. Available at: [https://less.works/less/technical-excellence](https://less.works/less/technical-excellence) (Accessed: 7 June 2025\)
\[27\] Thurlow, N., Turner, J.R. and Podder, A. (2020) The Flow System: The Evolution of Agile and Lean Thinking in an Age of Complexity（日本語訳版: フローシステムガイド）. Flow Consortium. Available at: [https://flowguides.org/Flow_Guide.pdf](https://flowguides.org/Flow_Guide.pdf) (Accessed: 17 May 2025).
\[28\] Felderer, M. and Travassos, G.H. (2020) 'The Evolution of Empirical Methods in Software Engineering'. Available at: [https://arxiv.org/pdf/1912.11512.pdf](https://arxiv.org/pdf/1912.11512.pdf) (Accessed: 17 May 2025).
\[29\] Creative Wisdom (n.d.) 'Abduction, Deduction and Induction'. Available at: [https://www.creative-wisdom.com/teaching/WBI/abduction5.pdf](https://www.creative-wisdom.com/teaching/WBI/abduction5.pdf) (Accessed: 17 May 2025).
\[30\] Blackburn, S. (2003) Ethics: A Very Short Introduction. Oxford: Oxford University Press.
\[31\] Cagan, M., 2018\. Inspired: How to Create Tech Products Customers Love. 2nd ed（日本語訳版: INSPIRED 熱狂させる製品を生み出すプロダクトマネジメント）. Hoboken, NJ: Wiley.
\[32\] Cagan, M. & Jones, C., 2020\. Empowered: Ordinary People, Extraordinary Products（日本語訳版: EMPOWERED 普通のチームが並外れた製品を生み出すプロダクトリーダーシップ）. Hoboken, NJ: Wiley.
\[33\] Cagan, M., 2024\. Transformed: Moving to the Product Operating Model（日本語訳版: TRANSFORMED イノベーションを起こし真のDXへと導くプロダクトモデル）. Hoboken, NJ: Wiley.
\[34\] Moore, G.A., 1991\. Crossing the Chasm: Marketing and Selling High-Tech Products to Mainstream Customers（日本語訳版: キャズム）. New York: Harper Business.
\[35\] Davies, Dan. (2025) The Unaccountability Machine: Why Big Systems Make Terrible Decisions—and How the World Lost Its Mind. London: Profile Books Ltd. (Paperback edition).
\[36\] Ackoff, R.L. (1999) Ackoff's Best: His Classic Writings on Management. New York: John Wiley & Sons.
\[37\] LeSS (n.d.) 'Why LeSS? Achieving adaptiveness'（日本語訳版: 何故 LeSSなのか?）. Available at: [https://less.works/less/framework/why-less](https://less.works/less/framework/why-less) (Accessed: 17 May 2025).
\[38\] Gothelf, J. & Seiden, J. (2021) Lean UX: Designing great products with agile teams. 3rd edn. Sebastopol, CA: O'Reilly Media
\[39\] Torres, T. (2021) Continuous discovery habits: Discover products that create customer value and business value. North Charleston, SC: Product Talk
\[40\] 'Genchi Genbutsu（現地現物）' (2024) Wikipedia. Available at: [https://en.wikipedia.org/wiki/Genchi_Genbutsu](https://en.wikipedia.org/wiki/Genchi_Genbutsu) (Accessed: 18 May 2025).
\[41\] van der Bles, A.M., van der Linden, S., Freeman, A.L.J. and Spiegelhalter, D.J. (2019) 'Communicating uncertainty about facts, numbers and science', Royal Society Open Science, 6(5), 181870\. Available at: [https://www.ncbi.nlm.nih.gov/pmc/articles/PMC6549952/](https://www.ncbi.nlm.nih.gov/pmc/articles/PMC6549952/) (Accessed: 17 May 2025).
\[42\] NetSuite (2023) 'What Is Business to Business to Consumer (B2B2C)?' Available at: [https://www.netsuite.com/portal/resource/articles/ecommerce/b2b2c.shtml](https://www.netsuite.com/portal/resource/articles/ecommerce/b2b2c.shtml) (Accessed: 17 May 2025).
\[43\] Dictionary Marketing (2024) 'B2B2B'. Available at: [https://dictionarymarketing.com/definition/b2b2b/](https://dictionarymarketing.com/definition/b2b2b/) (Accessed: 17 May 2025).
\[44\] Patton, J. and Economy, P. (2014) User Story Mapping: Discover the Whole Story, Build the Right Product（日本語訳版: ユーザーストーリーマッピング）. Sebastopol, CA: O'Reilly Media.
\[45\] Kotter, J.P., 1996\. Leading Change（日本語訳版: 企業変革力）. Boston: Harvard Business School Press.
\[46\] Csíkszentmihályi, M. (1990) Flow: The Psychology of Optimal Experience（日本語訳版: フロー体験 喜びの現象学）. New York: Harper & Row
\[47\] Stripe (2025) 'Sir Jony Ive and Patrick Collison Fireside Chat | Stripe Sessions 2025', YouTube video, 8 May. Available at: [https://youtu.be/wLb9g_8r-mE?si=1rEJxU0sxixvblQ3\&t=1390](https://youtu.be/wLb9g_8r-mE?si=1rEJxU0sxixvblQ3&t=1390) (Accessed: 8 June 2025\)
\[48\] Kanban Guides (2025)（日本語訳版: 2025年版カンバンガイド） Available at: [https://kanbanguides.org](https://kanbanguides.org/) (Accessed: 17 May 2025\)
\[49\] Scrum.org et al. (2021) The Kanban Guide for Scrum Teams（日本語訳版: スクラムチームのためのカンバンガイド）. Available at: [https://www.scrum.org/resources/kanban-guide-scrum-teams](https://www.scrum.org/resources/kanban-guide-scrum-teams) (Accessed: 17 May 2025\)
\[50\] Scotland, K. (2023) Why strategy deployment? Here are three great reasons, AvailAgility. At: [https://availagility.co.uk/2023/02/16/why-strategy-deployment-here-are-three-great-reasons/](https://availagility.co.uk/2023/02/16/why-strategy-deployment-here-are-three-great-reasons/) (Accessed: April 3, 2023).
\[51\] Scotland, K. (2019) Deploying strategies as choices, AvailAgility. At: [https://availagility.co.uk/2019/02/08/deploying-strategies-as-choices/](https://availagility.co.uk/2019/02/08/deploying-strategies-as-choices/) (Accessed: April 3, 2023).
\[52\] Scotland, K. (2017) Strategy deployment and playing to win, AvailAgility. At: [https://availagility.co.uk/2017/07/14/strategy-deployment-and-playing-to-win/](https://availagility.co.uk/2017/07/14/strategy-deployment-and-playing-to-win/) (Accessed: April 3, 2023).
\[53\] Scotland, K. (2017) A strategy deployment cadence, AvailAgility. At: [https://availagility.co.uk/2017/09/06/a-strategy-deployment-cadence/](https://availagility.co.uk/2017/09/06/a-strategy-deployment-cadence/) (Accessed: April 3, 2023).
\[54\] Scotland, K. (2022) The ultimate X-matrix for your agile transformation is here, AvailAgility. At: [https://availagility.co.uk/2022/11/03/the-ultimate-x-matrix-for-youragile-transformation-is-here/](https://availagility.co.uk/2022/11/03/the-ultimate-x-matrix-for-youragile-transformation-is-here/) (Accessed: April 5, 2023).
\[55\] Fuzzy Business: How to be roughly right rather than precisely wrong (unpublished).
\[56\] ScrumPlop, n.d. Illigitimus Non Interruptis. The Scrum Book: The Spirit of the Game. Available at: [https://sites.google.com/a/scrumplop.org/published-patterns/product-organization-pattern-language/illegitimus-non-interruptus](https://sites.google.com/a/scrumplop.org/published-patterns/product-organization-pattern-language/illegitimus-non-interruptus) \[Accessed: 18 May 2025\].
\[57\] Ohno, T. (1988) Toyota Production System: Beyond Large-Scale Production（日本語版: トヨタ生産方式 ― 脱規模の経営をめざして）. Portland, OR: Productivity Press.
\[58\] Toyota Motor Corporation (2024) Toyota Production System（日本語版: トヨタ生産方式）. Available at: [https://global.toyota/en/company/vision-and-philosophy/production-system/index.html](https://global.toyota/en/company/vision-and-philosophy/production-system/index.html) (Accessed: 17 May 2025).
\[59\] Hounshell, D.A. & Smith, J.K. (1988) Science and Corporate Strategy: DuPont R\&D, 1902–1980. Cambridge: Cambridge University Press.
\[60\] Schwaber, K. and Sutherland, J. (1995) 'SCRUM Development Process', OOPSLA Business Object Design and Implementation Workshop. Austin, Texas, October 1995\. Available at: [http://jeffsutherland.org/oopsla/schwapub.pdf](http://jeffsutherland.org/oopsla/schwapub.pdf) (Accessed: 17 May 2025).
\[61\] Members of The Scrum Patterns Group: Vervloed, E., Harrison, N., Harada, K., Yoder, J., Kim, J., O'Callaghan, A., Beedle, M., Bjørnvig, G., Friis, D., Reijonen, V., Benefield, G., Østergaard, J., Eloranta, V.-P., Leonard, E. & Aguiar, A.
\[62\] Boyd, J.R. (1995–1996) The Essence of Winning and Losing. Unpublished briefing slides. Note: Boyd's OODA was primarily disseminated through military briefings and unpublished manuscripts. His final conceptualization appears in The Essence of Winning and Losing, which emphasizes nonlinear decision-making and adaptation in complex environments.
\[63\] Turner, J.R., Thurlow, N. and Rivera, B. (2019) The Flow System Guide（日本語訳版: フローシステムガイド）. Available at: [https://flowguides.org/Flow_Guide.pdf](https://flowguides.org/Flow_Guide.pdf) (Accessed: 24 May 2025). 要約：このガイドはBoydのOODAを複雑性理論とアジャイル実践と統合し、組織のフローのための動的で非線形な意思決定プロセスとして枠組み化している。
