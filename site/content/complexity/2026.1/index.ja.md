---
# title: Complexity (Expansion of the SGEP)
title: 複雑性（SGEP拡張版）
# subtitle: Cynefin Framework Kind of Explanation unofficial & unauthorized
subtitle: クネビンフレームワーク 勝手に非公式解説
# description: Understand why product development fails when teams apply one fixed process to every situation. This guide explains complexity through the Cynefin Framework and shows how different contexts demand different responses. It clarifies why Scrum works best in complex, liminal spaces, where stability and experimentation coexist, helping leaders and teams sense change early, avoid fragile certainty, and adapt their way of working as patterns emerge.
description: チームがすべての状況に固定化したプロセスを適用するとき、なぜプロダクト開発が失敗するかを理解する。このガイドはクネビンフレームワークを通じて複雑性を説明し、異なる文脈が異なる対応を要求することを示す。スクラムが複雑でリミナルな空間、つまり安定性と実験が共存する場所で最も効果を発揮する理由を明確にし、リーダーとチームが変化を早期に察知し、脆弱な確実性を避け、パターンが創発するにつれて働き方を適応させることを支援する。
# keywords:
#   - Complexity
#   - Cynefin
#   - Empirical learning
#   - Liminality
keywords:
  - 複雑性
  - クネビン
  - 経験的学習
  - リミナリティ
author:
  - Ralph Jocham
  - John Coleman
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
  - /ja/complexity/2026.1/
---

<!-- ***Collected Resources for Scrum Guide Expansion Pack*** -->

**_スクラムガイド拡張パック収録資料_**

<!-- *This document is a collection of independent works. Each section retains its original license or copyright status, as indicated. Please refer to each section for specific usage rights and requirements.* -->

_本書は、独立した著作物を収録したものである。各セクションは記載の通り、オリジナルのライセンスや著作権状況を保持している。特定の使用権限と要件については、各セクションを参照して欲しい。_

<!-- *License: Creative Commons Attribution-ShareAlike 4.0 International ([CC BY-SA 4.0](https://creativecommons.org/licenses/by-sa/4.0/)).* © 2017-*2025 Cynefin.io.* -->

_ライセンス：クリエイティブ・コモンズ 表示-継承 4.0 国際（[CC BY-SA 4.0](https://creativecommons.org/licenses/by-sa/4.0/)）。 © 2017-2025 Cynefin.io._

<!-- *Disclaimer: No warranties are given. Use at your own risk.* -->

_免責事項：いかなる保証も提供されない。ご自身の責任で使用されたい。_

<!-- *This section is offered under the Attribution-ShareAlike 4.0 International license of Creative Commons.* -->

_このセクションは、クリエイティブ・コモンズの表示-継承4.0国際ライセンスの下で提供されている。_

<!-- *By using this Cynefin Framework Kind of Explanation unofficial & unauthorized, you agree to the terms of the [CC BY-SA 4.0](https://creativecommons.org/licenses/by-sa/4.0/) license.* -->

_このクネビンフレームワーク 勝手に非公式解説を使用することで、[CC BY-SA 4.0](https://creativecommons.org/licenses/by-sa/4.0/)ライセンスの条項に同意したものとみなされる。_

---

<!-- ## Cynefin® -->

## クネビン（Cynefin®） {#cynefin}

<!-- Cynefin® \[1-6\] offers a compass for leadership decision-making. It was popularized by the HBR article 'A Leader's Framework for Decision Making' by Dave Snowden and Mary Boone in 2007 and again in 'Managing complexity (and chaos) in a crisis \- a field guide for decision makers inspired by the Cynefin framework', also known as the 'EU Field Guide.' Its premise is that one should act differently depending on the dynamics of the space. It is often oversimplified. A given problem could exist in all domains simultaneously, each having different aspects. -->

クネビン（Cynefin®）[1-6]は、リーダーシップの意思決定のための羅針盤を提供する。これは2007年のDave SnowdenとMary BooneによるHBR論文「意思決定のためのリーダーのフレームワーク」と、「EUフィールドガイド」としても知られる「危機における複雑性（と混沌）の管理 ～クネビンフレームワークに着想を得た意思決定者のためのフィールドガイド」によって普及した。その前提は、各領域の力学に応じて取るべき行動は異なる、ということである。これはよく、単純化されすぎてしまう。ある問題は、すべてのドメインに同時に存在しながら、別の特性を持つ可能性がある。

<!-- A phase shift refers to an often abrupt transition between domains, particularly from the ordered to chaos, triggered when a system's constraints (rules, habits, boundaries, and feedback) are misaligned or collapse. It marks a fundamental change in system behavior where previous methods of control or understanding no longer work. -->

位相シフトとは、しばしば発生する、ドメイン間の急激な移行のことである。特に秩序から混沌への移行において、システムの制約（ルール、習慣、境界、フィードバック）が不整合を起こしたり崩壊したりした時に引き起こされる。これは、システム行動の根本的変化を示すものであり、これまでの統制や理解の方法がもはや機能しなくなる状況である。

<!-- Not all aspects of Product development are complex. The Scrum Team, for a given situation, might need to consider a variety of phase shifts between: -->

プロダクト開発のすべての側面が複雑であるわけではない。スクラムチームは、特定の状況において、以下の間の様々な位相シフトを考慮する必要があるかもしれない：

<!-- - Ordered: Key idea: Stability, routine, best/good practice, expertise
  - Expertise is sufficient, and cause and effect are predictable or knowable
  - Response options not limited to: Apply best/good practices, follow rules, use expert analysis, do individual research
  - Metaphors: Hard to barely frozen ice cube, pleasant weather, or chess/sudoku
  - Nature example: A modern, climate-controlled glasshouse--predictable, controlled, planned growth
  - Product example: Resolving a tricky technical issue by consulting experts and analyzing logs -->

- 秩序：主要概念：安定性、ルーチン、ベスト/グッドプラクティス、専門知識
  - 専門知識で十分であり、原因と結果は予測可能または認識可能
  - 対応選択肢（これらに限定されない）：ベスト/グッドプラクティスの適用、ルールの遵守、専門家分析の活用、個別調査の実施
  - 比喩：硬い氷からかろうじて凍った氷まで、快適な天気、チェス/数独
  - 自然の例：現代の気候制御された温室——予測可能で統制された計画的成長
  - プロダクトの例：専門家への相談とログ分析により困難な技術的問題を解決する

<!-- - Complex \[1-6\], where expertise is valuable but not enough, and one can only understand why things happened after the fact. Key idea: emergence, safe-to-fail experiments
  - Responses not limited to:
    - Encourage learning and adaptation
    - Trying several small, parallel, safe-to-fail experiments
    - Fostering fresh thinking through cognitive diversity and collaboration
    - Borrowing solutions from other places if they might help
    - Testing out smart guesses or informed hunches to see what works
  - This is all while following helpful guidelines that encourage good results to develop naturally
  - Metaphors: Flowing water, rainy weather, or poker
  - Nature example: Bramble thicket--everything is entangled, connections are unpredictable
  - Product example: Experimenting with different features or solutions informed by user feedback, e.g., A/B testing new Product ideas -->

- 複雑[1-6]：専門知識は価値があるが不十分で、なぜ物事が起こったかは事後にのみ理解できる。主要概念：創発、失敗しても安全な実験
  - 対応（これらに限定されない）：
    - 学習と適応を促す
    - いくつかの小さな並行した失敗しても安全な実験を試す
    - 認知的多様性と協働を通じて新鮮な思考を育む
    - 役立つ可能性がある場合は他の場所からソリューションを借用する
    - 何が機能するかを確認するために賢明な推測や情報に基づく直感をテストする
  - これらはすべて、良い結果が自然に発展することを促す有益なガイドラインに従いながら行う
  - 比喩：流れる水、雨天、ポーカー
  - 自然の例：茨の茂み —— すべてが絡み合い、つながりは予測不可能
  - プロダクトの例：ユーザーフィードバックに基づく異なるフィーチャーやソリューションの実験、例：新しいプロダクトアイデアのA/Bテスト

<!-- - Chaotic:
  - Negative: Key idea: Destructive crisis, breakdown, urgent action
    - Responses not limited to: Take immediate action to restore order, prioritize safety, do something quickly without making matters worse
    - Metaphors: Shattering ice or uncontrolled explosion, toxic gas, tornado, earthquake, wildfire, or a riot in a stadium
    - Nature example: Natural disaster (e.g., tsunami)–sudden, destructive, unpredictable
    - Product example: Responding to a critical security breach by isolating systems and deploying emergency fixes
  - Positive: Key idea: Generative disruption, rapid innovation
    - Response options not limited to: Disrupt intentionally, encourage creativity, harness energy, e.g., hackathon, incubator, 'Innovation Friday'
    - Metaphors: Controlled explosion (steam engine), fireworks, or festival bonfire
    - Nature example: Forest fire clearing old growth for new plants–ecosystem renewal
    - Product example: Rapidly pivoting a Product during a market disruption to seize new opportunities (e.g., launching a feature in response to a competitor's move) -->

- 混沌：
  - 負の場合：主要概念：破壊的危機、破綻、緊急行動
    - 対応（これらに限定されない）：秩序回復のための即座の行動、安全の優先、事態を悪化させることなく迅速に何かを行う
    - 比喩：砕ける氷や制御されない爆発、毒ガス、竜巻、地震、山火事、スタジアムでの暴動
    - 自然の例：自然災害（例：津波） —— 突然で、破壊的で、予測不可能
    - プロダクトの例：システムを隔離し緊急修正を展開することで重大なセキュリティ侵害に対応する
  - 正の場合：主要概念：生成的破壊、急速なイノベーション
    - 対応選択肢（これらに限定されない）：意図的に破壊し、創造性を促し、エネルギーを活用する、例：ハッカソン、インキュベーター、「イノベーション・フライデー」
    - 比喩：制御された爆発（蒸気機関）、花火、祭りのかがり火
    - 自然の例：新しい植物のために古い成長を取り除く森林火災 —— 生態系の更新
    - プロダクトの例：新しい機会を捉えるために市場の混乱中にプロダクトを急速にピボットする（例：競合他社の動きに対応してフィーチャーを立ち上げる）

<!-- Liminality is an 'in-between' stage, like a threshold. The often less-sudden phase shifts happen in the liminals: -->

リミナリティ（境界状況）とは「中間」段階、閾値のようなものである。それほど突然でない位相シフトは、しばしばそのリミナル（境界）で起こる：

<!-- - In the liminal between complex and ordered, this is Scrum's default sweetspot:
  - Ordered-Complex:
    - From expert analysis to adaptive exploration
    - Responses not limited to: Relax some rules, introduce experimentation, prepare for emergence
    - Metaphors: A melting ice cube, cloudy weather, switching from chess to poker
    - Nature example: Seasonal thaw–rigid ice giving way to flowing streams and new growth
    - Product example: When a routine process stops working, encourage the team to try different approaches
  - Complex-Ordered:
    - Responses not limited to: Turn creative discoveries into expert routines; stabilize innovation, observe and codify successful patterns; transition to standardization
    - Metaphors: Slush (between ice and water), fog lifting after rain, switching from poker to chess
    - Nature example: River delta forming channels–from unpredictable to stable flows
    - Product example: Taking a successful experimental feature and turning it into a documented, repeatable process -->

- 複雑と秩序の間のリミナル。これはスクラムが最も得意とする領域である：
  - 秩序——複雑：
    - 専門家分析から適応的探索へ
    - 対応（これらに限定されない）：いくつかのルールを緩和し、実験を導入し、創発に備える
    - 比喩：溶ける氷、曇り天気、チェスからポーカーへの切り替え
    - 自然の例：季節の解凍 —— 硬い氷が流れる小川と新しい成長に道を譲る
    - プロダクトの例：ルーチンプロセスが機能しなくなったとき、チームに異なるアプローチを試すよう促す
  - 複雑——秩序：
    - 対応（これらに限定されない）：創造的発見を専門家ルーチンに変換し、イノベーションを安定化し、成功パターンを観察・体系化し、標準化に移行する
    - 比喩：みぞれ（氷と水の間）、雨後の霧の晴れ間、ポーカーからチェスへの切り替え
    - 自然の例：水路を形成する川のデルタ —— 予測不可能から安定した流れへ
    - プロダクトの例：成功した実験的フィーチャーを文書化された再現可能なプロセスに変換する

<!-- - In the liminal between complex and chaotic:
  - Complex–Chaotic (positive):
    - A situation where constraints need to be relaxed to create time and space for innovation or invention. Key idea: The edge of creativity, risk, and innovation
    - Responses not limited to: Loosen constraints, encourage experimentation, seek breakthrough ideas
    - Metaphors: Boiling water (on the edge of steam), thunderstorm breaking out, Improvizational theater, or jazz jam session
    - Nature example: Volcano creating new land–creative transformation at the edge of chaos
    - Product example: Running a high-risk innovation hackathon to generate disruptive ideas
  - Complex–Chaotic (negative):
    - Key idea: A destructive move into crisis
    - Responses not limited to: Rapidly re-impose constraints, stabilize the situation, prevent further breakdown
    - Metaphors: Exploding pressure cooker, sudden tornado or flash flood, game pieces thrown in anger, game board upended
    - Nature example: Sudden landslide–loss of structure, destructive transition
    - Product example: Failed Product launch confusion, and urgent need to regain control
  - Chaotic-Complex: Getting out of chaotic--regrouping
    - Response options not limited to: Sense emerging order, start probing, encourage collaboration, and pattern recognition
    - Metaphors: Steam condensing to water, calm after a hurricane, restarting a sports game after a storm
    - Nature example: Pioneer species colonizing after fire–new growth after disturbance
    - Product example: After a crisis, regrouping the team to experiment with new ways of working or new Product directions -->

- 複雑と混沌の間のリミナル：
  - 複雑——混沌（正）：
    - イノベーションや発明のための時間と空間を作るために制約を緩和する必要がある状況。主要概念：創造性、リスク、イノベーションの端
    - 対応（これらに限定されない）：制約を緩め、実験を促し、ブレークスルーのアイデアを求める
    - 比喩：沸騰する水（蒸気の端で）、発生する雷雨、即興劇場、ジャズジャムセッション
    - 自然の例：新しい土地を創造する火山 —— 混沌の端での創造的変革
    - プロダクトの例：破壊的アイデアを生成するための高リスクイノベーションハッカソンの実行
  - 複雑——混沌（負）：
    - 主要概念：危機への破壊的移行
    - 対応（これらに限定されない）：制約を急速に再課し、状況を安定化し、さらなる破綻を防ぐ
    - 比喩：爆発する圧力鍋、突然の竜巻や鉄砲水、怒りで投げられたゲームの駒、ひっくり返されたゲーム盤
    - 自然の例：突然の地すべり —— 構造の喪失、破壊的移行
    - プロダクトの例：失敗したプロダクト立ち上げの混乱と、統制を取り戻す緊急の必要性
  - 混沌——複雑：混沌からの脱出 —— 再編成
    - 対応選択肢（これらに限定されない）：創発する秩序を感知し、探索を開始し、協働を促し、パターン認識を行う
    - 比喩：水に凝縮する蒸気、ハリケーンの後の静寂、嵐の後のスポーツゲームの再開
    - 自然の例：火災後に移住する先駆種 —— 攪乱後の新しい成長
    - プロダクトの例：危機の後、新しい働き方や新しいプロダクト方向を実験するためのチームの再編成

<!-- - Aporia (paradoxical liminal): sitting with paradox for new insight, perhaps after realizing the situation at hand was not as it seemed
  - Response options: Hold ambiguity, encourage reflection, allow new understanding to emerge
  - Metaphors: Triple point (solid, liquid, gas coexist), standing in the eye of a storm, solving a riddle
  - Nature example: Estuary where river, sea, and land meet–all states and possibilities coexist
  - Product example: The team is stuck between conflicting strategies or visions and should briefly pause to reflect and realign. -->

- アポリア（逆説的リミナル）：新しい洞察のために逆説と共に向き合う。おそらく目前の状況が見えていたものと異なることを悟った後に。
  - 対応選択肢：曖昧さを保持し、振り返りを促し、新しい理解の創発を可能にする
  - 比喩：三重点（固体、液体、気体が共存）、嵐の目の中に立つ、謎かけを解く
  - 自然の例：川、海、陸が出会う河口——すべての状態と可能性が共存する
  - プロダクトの例：チームが対立する戦略やビジョンの間で行き詰まり、振り返りと再整合のために短時間立ち止まるべき状況。

<!-- - A rarely considered phase shift due to difficulty level: Chaotic-Orderly liminal
  - Response options: Impose strong constraints, re-establish rules and structure
  - Metaphors: Ice rapidly refreezing, cold snap after a storm, referee is successfully strict after chaos
  - Nature example: A Dam is successfully built after a flood--a wild river suddenly contained and controlled
  - Product example:
    - After a major production outage or Product crisis, a cross-functional crisis team rapidly stabilizes the situation with clear, minimal rules and temporary protocols
    - Once the immediate danger is past, these are iteratively refined and formalized into sustainable, balanced processes, avoiding overcorrection or excessive bureaucracy -->

- 困難度のため稀に考慮される位相シフト：混沌——秩序リミナル
  - 対応選択肢：強い制約を課し、ルールと構造を再確立する
  - 比喩：急速に再凍結する氷、嵐の後の寒波、混沌の後に審判が効果的に厳格さを取り戻す
  - 自然の例：洪水の後にダムが成功裏に建設される —— 荒々しい川が突然封じ込められ統制される
  - プロダクトの例：
    - 大規模な本番障害またはプロダクト危機の後、機能横断的危機チームが明確で最小限のルールと一時的プロトコルで状況を急速に安定化させる
    - 直近の危険が過ぎると、これらは持続可能でバランスの取れたプロセスへと反復的に洗練・正式化され、過剰修正や過度な官僚主義を回避する

<!-- One phase shift is particularly sudden and negative, that is, the ordered-chaotic liminal:
- Response options: Recognize fragility and over-confidence, act quickly to restore boundaries and safety
- Metaphors: Ice cracking into shards, sudden and violent hailstorm, game rules suddenly thrown out
- Nature example: Frozen lake breaking up in spring--stable surface suddenly shattering
- Product example: A stable Product process suddenly breaks down due to an unexpected event (e.g., major outage) -->

特に突然で負の位相シフトが一つある、それは秩序-混沌リミナルである：
- 対応選択肢：脆弱性と過信を認識し、境界と安全を回復するために迅速に行動する
- 比喩：破片に割れる氷、突然で激しい雹嵐、ゲームのルールが突然破棄される
- 自然の例：春に崩壊する凍った湖 —— 安定した表面が突然砕け散る
- プロダクトの例：予期しない事象（例：大規模な障害）のために安定したプロダクトプロセスが突然破綻する

<!-- ## Attribution for the Scrum Guide Expansion Pack Collection -->

## スクラムガイド拡張パックにおける収録資料の帰属情報 {#attribution-for-the-scrum-guide-expansion-pack-collection}

<!-- This collection was written and compiled by *Ralph Jocham, John Coleman, and Jeff Sutherland*. Each section is individually attributed above and retains its original license. The collection as a whole is for informational purposes; please respect the license terms of each section. -->

このコレクションは、_Ralph Jocham、John Coleman、Jeff Sutherland_ によって執筆・編纂された。各セクションは上記で個別に帰属が示されており、オリジナルのライセンスを保持している。コレクション全体は情報提供を目的としている。各セクションのライセンス条項を尊重して欲しい。

<!-- ## References -->

## 参考文献 {#references}

\[1\] [Cynefin.io](https://Cynefin.io/), V. (2022) Cynefin wiki, [Cynefin.io](https://Cynefin.io/). [Cynefin.io](https://Cynefin.io/). At: [https://cynefin.io/](https://cynefin.io/) (Accessed: April 4, 2023).
\[2\] Rancati, A. and Snowden, D. (2021) Managing complexity (and chaos) in a crisis \- a field guide for decision makers inspired by the Cynefin framework. Luxembourg, Belgium: Publications Office of the European Union.
\[3\] Snowden, D. et al. (2022) Cynefin® weaving sense-making into the fabric of our world. 2nd edn. Edited by R. Greenberg and B. Bertsch. Singapore, Singapore: Cognitive Edge \- The Cynefin Co.
\[4\] Snowden, D. (2023) Cynefin St David's 2023 1 of 2, Cynefin Co. [https://thecynefin.co/cynefin-st-davids-2023-1-of-2/](https://thecynefin.co/cynefin-st-davids-2023-1-of-2/) (Accessed: April 20, 2023).
\[5\] Snowden, D. (2023) Managing for emergence through abduction, The Cynefin Co. At: [https://thecynefin.co/managing-for-emergence/](https://thecynefin.co/managing-for-emergence/) (Accessed: June 24, 2023).
\[6\] Snowden, D. and Smith, N. (2023) Leadership discussion: Dave and Natalie \- the Cynefin co, YouTube. At: [https://youtu.be/WcPZ8ybDF0w](https://youtu.be/WcPZ8ybDF0w) (Accessed: April 7, 2023).
