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
