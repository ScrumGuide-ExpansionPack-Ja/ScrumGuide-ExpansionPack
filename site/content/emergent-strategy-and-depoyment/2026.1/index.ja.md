---
# title: Emergent Strategy (Expansion of the SGEP)
title: 創発的戦略（SGEP拡張版）
# description: The Scrum Guide Expansion Pack is a comprehensive companion to the 2020 Scrum Guide, created to help professionals navigate today's complex product environments. It deepens understanding of core Scrum principles by offering additional guidance on complexity, product thinking, systems of work, and leadership; while remaining true to Scrum's ethos of empiricism and self-management. It's not a rewrite, but a strategic amplification to support long-term, value-driven delivery in modern teams.
description: スクラムガイド拡張パックは、今日の複雑なプロダクト環境を渡り歩く専門家を支援するために作成された、2020スクラムガイドの包括的な補完資料である。複雑性、プロダクト思考、作業システム、リーダーシップに関する追加のガイダンスを提供することで、スクラムの核心となる原則の理解を深める。経験主義と自己管理というスクラムの精神に忠実でありながら、現代のチームにおける長期的で価値駆動型のデリバリーを支援するための戦略的増幅である。
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
  - 複雑な環境におけるスクラム
  - スクラムとAI
author:
  - Roger L. Martin
  - Tom Gilb
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
  priority: 0.7
aliases:
  - /ja/emergent-strategy-and-depoyment/2026.1/
---

<!-- ***Collected Resources for Scrum Guide Expansion Pack*** -->

**_スクラムガイド拡張パック収録資料_**

<!-- *This document is a collection of independent works. Each section retains its original license or copyright status, as indicated. Please refer to each section for specific usage rights and requirements.* -->

_本書は、独立した著作物を収録したものである。各セクションは記載の通り、オリジナルのライセンスや著作権状況を保持している。特定の使用権限と要件については、各セクションを参照して欲しい。_

<!-- Copyright: All rights reserved. Adapted -->

著作権：無断転載禁止。適応版

---

<!-- Strategy is not limited by scale; if it exists, it should be clearly articulated at the corporate, business unit, or Product level and remain coherent and integrated across these levels. Crucially, strategy should distinguish between ends (quantified, Stakeholder-valued outcomes) and means (initiatives or activities). -->

戦略は規模によって制限されるものではなく、存在するのであれば、企業全体、事業部門、あるいはプロダクトレベルにおいて明確に表現されていなければならない。さらに、これらのレベル間で一貫性を保ち統合されているべきである。重要なのは、戦略が目的（定量化されたステークホルダーにとって価値のあるアウトカム）と手段（施策や活動）を区別していることである。

<!-- Drawing from and adapting Roger L. Martin's work (1) and Tom Gilb's work (3-8), strategy is about making integrated, explicit choices- deciding what and what not to pursue from a well-defined, measurable winning aspiration, not just a broad mission or vision. Effective strategy answers: -->

Roger L. Martinの著作[1]とTom Gilbの著作[3-8]を参考にし、適応すると、戦略とは統合された明示的な選択を行うことである。つまり、単なる広範なミッションやビジョンではなく、明確に定義され計測可能な達成すべき成功目標から、何を追求し何を追求しないかを決定することである。効果的な戦略は以下の問いに答えるものである：

<!-- - Where will we play?
- How will we win ethically (9) and sustainably, balancing a multiplicity of expectations and limits?
- What capabilities and systems must be in place?
- What else must be true for this strategy to succeed? -->

- どの領域で勝負するのか？
- 倫理的[9]かつ持続可能な形で、複数の期待と制約のバランスを取りながら、いかにして勝つのか？
- どのような能力とシステムが備わっていなければならないのか？
- この戦略が成功するために、他にどのような前提条件が成立していなければならないのか？

<!-- For situations where expertise alone is sufficient (or perhaps bordering on being sufficient), to ensure strategy is iterative, actionable, and value-focused: -->

専門知識だけで十分である（あるいは、ほぼ十分である）状況においても、戦略を反復的・実行可能・価値志向にするためには以下が不可欠である：

<!-- - Iteratively quantify and manage Stakeholder value, multiple impacts or side effects, risks, and trade-offs:
  - Identify all critical Stakeholders (including but not limited to customers) and define their value objectives in measurable terms (e.g., 'reduce new-user onboarding time from 5-10 to 2-4 days').
  - Explicitly quantify trade-offs and constraints, and revisit as new information emerges.
  - Use integrative thinking to resolve tensions creatively. -->

- ステークホルダー価値、複数の影響や副作用、リスク、トレードオフを反復的に定量化し管理する：
  - すべての重要なステークホルダー（顧客を含むがこれに限定されない）を特定し、それぞれの価値目標を計測可能な形で定義する（例：「新規ユーザーのオンボーディング時間を5〜10日から2〜4日に短縮する」）。
  - トレードオフと制約を明示的に定量化し、新しい情報が得られるたびに見直す。
  - 統合的思考を用いて緊張関係を創造的に解決する。

<!-- - Co-create and prioritize collaboratively:
  - Develop the strategy by blending top-down and bottom-up insights and lateral collaboration.
  - Use structured workshops and feedback loops to foster alignment and adaptability, and continuously reprioritize unstarted work. -->

- 共創し、協働で優先順位づけする：
  - トップダウン・ボトムアップの洞察・横断的なコラボレーションを融合して戦略を策定する。
  - 構造化されたワークショップとフィードバックループを活用して整合性と適応性を促進し、未着手の作業の優先順位を継続的に見直す。

<!-- - Deliver value incrementally and measure results:
  - Iteratively break down strategic aspirations into small, prioritized, measurable increments.
  - Deliver value in short cycles (e.g., Sprints or weeks), measuring actual outcomes and side effects against original quantified objectives.
  - Use regular reviews to adjust informed by real-world feedback. -->

- 価値を漸進的に提供し、結果を計測する：
  - 戦略的志向を、小さく優先順位づけされた計測可能なインクリメントに反復的に分解する。
  - 短いサイクル（例：スプリントや週単位）で価値を提供し、実際のアウトカムと副作用を当初定量化した目標と照らし合わせて計測する。
  - 定期的なレビューを活用し、現実のフィードバックに基づいて調整する。

<!-- - Enable emergence:
  - Allow strategy to evolve in response to new data and Stakeholder (including but not limited to user) feedback, within a framework of clear, quantified objectives, measurable trends, and regular risk/benefit reassessment.
  - Make course corrections rapidly and transparently as reality unfolds. -->

- 創発を可能にする：
  - 明確に定量化された目標、計測可能なトレンド、定期的なリスク・恩恵再評価という枠組みの中で、新たなデータやステークホルダー（ユーザーを含むがこれに限定されない）のフィードバックに応じて戦略が進化することを許容する。
  - 現実の展開に応じて、迅速かつ透明に軌道修正を行う。

<!-- - Ensure strategy and strategy deployment are outcome-oriented and focused (deciding what to and what not to work on). Distinguish between:
  - Strategy including the intent, rationale, goals, and anti-goals (the _what_ and _why_),
  - Strategy deployment: the operationalization of the strategy, iterative sequencing or decomposition of integrated choices for the strategy, usually in small outcome-oriented slices of the _what_ and _why_,
  - Outcome-oriented, focused Product Backlog Items (smaller slices for _whom_), and
  - Lists of activities or initiatives (the 'what we'll do' or _how_).
- Avoid mistaking a collection of projects for a coherent, value-driven strategy. -->

- 戦略と戦略展開をアウトカム指向で焦点の定まったものにする（何に取り組み、何に取り組まないかを決定）。以下を区別する：
  - 戦略：意図、根拠、ゴール、避けるべきゴール（_何を_、_なぜ_）
  - 戦略展開：戦略の運用化。戦略のための統合された選択肢の反復的な配列・分解。通常は _何を_、_なぜ_ の小さなアウトカム指向スライス
  - アウトカム指向で焦点の定まったプロダクトバックログアイテム（_誰のために_ による、より小さなスライス）
  - 活動や施策のリスト（「何をやるか」または _どのように_）
- プロジェクトの寄せ集めを、一貫性ある価値駆動戦略と間違えないこと。

<!-- For situations where expertise is valuable yet insufficient, cause and effect are only coherent in retrospect, and uncertainty needs to be embraced, Scrum Teams and Stakeholders need to: -->

専門知識には価値があるがそれだけでは不十分であり、因果関係が後になって初めて一貫していることがわかるような状況では、不確実性を受け入れる必要がある。スクラムチームとステークホルダーは次のように取り組む必要がある：

<!-- - Embrace the messiness of less structured and emergent outcome-oriented work in a direction of travel.
- Consider that detailed, long-term plans are ineffective. Instead, organizations should focus on creating conditions where useful patterns and innovations can emerge from interactions within the system.
- Instead of trying one idea at a time and sticking to what worked before, Scrum Teams should consider several small, parallel safe-to-fail experiments at once to see what happens and learn from what emerges.
- Foster a climate for creative exploration, innovation, and evolution from the present. Create processes and environments where people can connect novel ideas, learnings, informed hunches, and learn from each other, rather than imposing uniformity or rigid KPIs. -->

- 進むべき方向性において、構造が定まっていない創発的なアウトカム指向の作業での混乱を受け入れる。
- 詳細かつ長期的な計画は効果的でないことを考慮する。その代わりに、組織はシステム内の相互作用から有用なパターンやイノベーションが創発するような条件を整えることに注力すべきである。
- 一度に一つのアイデアを試し、以前にうまくいったことに固執するのではなく、スクラムチームは、同時にいくつかの失敗しても安全な小さな実験を並行して行い、その結果を観察し、そこから学ぶべきである。
- 創造的な探索、イノベーション、現在からの進化を促す風土を促進する。人々が新しいアイデア、学び、情報に基づく直感を結びつけ、お互いから学び合えるプロセスと環境を創出する。均一性や硬直化したKPIを押し付けるべきではない。

<!-- - Response options are not restricted to:
  - Map what is already known and understand the system's evolutionary potential before attempting change
  - Foster self-organization
  - Run safe-to-fail experiments (probes)–probes should be small, parallel, and designed so that failure is survivable and informative
  - Seek fresh thinking
  - Try solutions for different problems for the current situation at hand
  - Test educated hunches
  - Observe what emerges, and amplify successful patterns while dampening or stopping those that don't work
  - Innovation is important, but proven solutions should be reused for recurring problems
  - Continuously sense-make
  - Perform narrative capture -->

- 対応策は以下に限定されない：
  - 変化を試みる前に、既知のことをマッピングし、システムの進化の可能性を理解する
  - 自己組織化を促進する
  - 失敗しても安全な実験（プローブ）を実行する —— プローブは小さく、並行して、失敗しても許され、有益な情報となるように設計されるべき
  - 新鮮な思考を求める
  - 目前の現在の状況について、異なる問題に対する解決策を試す
  - 根拠に基づく直感を試す
  - 何が創発するのかを観察し、うまくいくパターンは強化し、機能しないものは抑制または停止する
  - イノベーションは重要だが、繰り返し現れる問題に対しては、実証された解決策を再利用する
  - 継続的にセンスメイキングを行う
  - ナラティブキャプチャを実行する

<!-- - Metaphor: The role of leaders is to actively prepare and manage the soil, boundaries, and conditions (the 'substrate') to encourage the growth of healthy plants (emergent solutions). This includes metaphorically weeding, pruning, and shaping the environment, not just passively waiting for results. -->

- 比喩：リーダーの役割は、健全な植物（創発的な解決策）の成長を促進するために土壌、境界、条件（「基質」）を積極的に準備し管理することである。これには比喩的な除草、剪定、環境整備も含まれ、単に受動的に結果を待つのではない。

<!-- Generally, extrinsic motivation rewards should be avoided due to the 'cobra effect' (10) unless they are coherent with Beyond Budgeting. Equally, individual or team performance should be uncoupled from results as results might have been delivered, but in what way were they delivered, with what side effects, and what impact did delivery have on team morale, etc? -->

一般的に、外発的動機づけによる報酬は「コブラ効果」[10]を招く恐れがあり、脱予算経営の理念と整合性が取れない限りは避けるべきである。同様に、個人やチームのパフォーマンスは結果から切り離して考えるべきである。なぜなら、結果は達成されたとしても、それがどのような方法で達成されたのか、どのような副作用があったのか、チームの士気にどのような影響を与えたのかといった要素が関係しているからだ。

<!-- Nevertheless:
- There is disagreement in peer-reviewed papers (11-14) and a foundational non-peer-reviewed paper (15) on whether quantifying Stakeholder expectations, Stakeholder limits, or goals is helpful or unhelpful and whether it reduces intrinsic motivation.
- Consider the context. Also, consider whether quantification supports autonomy and meaning or imposes controlling constraints.
- For now, this document prefers to err on the side of clarification and shared understanding of an idea, quantifying Stakeholder expectations, Stakeholder limits, and the direction of travel, supported by high-quality and accurate storytelling narratives (more stories like this, fewer stories like that). -->

それでもなお、以下の点に留意すべきである：

- ステークホルダーの期待、ステークホルダーの制約、または目標を定量化することが有用か有害か、また内発的動機を低下させるかについて、査読付き論文[11-14]と基礎的な非査読論文[15]の間で意見の相違がある。
- 文脈を考慮すること。また、定量化が自律性や意味付けを支援するものか、統制的制約を課すものかを考慮すること。
- 現時点で、この文書はアイデアの明確化と共有理解を重視する立場を取る。すなわち、ステークホルダーの期待、ステークホルダーの制約、進むべき方向性を定量化し、高品質で正確なストーリーテリングナラティブ（このようなストーリーを増やし、あのようなストーリーを減らす）で補完することを推奨する。

<!-- An Emergent Strategy is supported by an emergent outcome-oriented roadmap, which can range from the Sprint Goal to the Product Vision and beyond. Emergent Strategy Deployment (16-19) should not be confused with Emergent Strategy. Vector change models (30-35, 54\), Product Operating Models (20-26), scaling and descaling models (27-40), and emergent goal-oriented models (16-19, 41-50) can be highly beneficial for Emergent Strategy Deployment. Err on the side of models coherent with vector-change, e.g., direction of travel over fixed goals. -->

創発的戦略は、スプリントゴールからプロダクトビジョン、さらにはその先に至るまでの、創発的かつアウトカム指向のロードマップによって支えられる。創発的戦略の展開[16-19]は創発的戦略そのものと混同するべきではない。ベクトル変化モデル[30-35,54]、プロダクトオペレーティングモデル[20-26]、スケーリングおよびデスケーリングモデル[27-40]、創発的ゴール指向モデル[16-19,41-50]は、創発的戦略の展開において非常に有益となりうる。あらかじめ固定した目標よりも進むべき方向性を重視するような、ベクトル変化と一貫性のあるモデルを採用することが望ましい。

<!-- Emergent strategy deployment involves allowing plans and actions to develop naturally as the Scrum Team and Stakeholders respond to real-world changes. Instead of following a fixed path, they pay attention to what is happening around them and make adjustments as they go. Over time, the steps taken form a pattern that becomes the actual strategy, even if it differs from what was initially intended. -->

創発的戦略の展開は、スクラムチームおよびステークホルダーが現実世界の変化に対応する中で、計画と行動が自然に展開していくのを可能にすることを意味する。あらかじめ固定された道筋に従うのではなく、周囲で起きていることに注意を払いながら、状況に応じて調整を行う。そうして時間をかけて、取られたステップがたとえ当初意図したものと異なっていたとしても、実際の戦略となるパターンを形成するのである。

<!-- ## Attribution for the Scrum Guide Expansion Pack Collection -->

## スクラムガイド拡張パックにおける収録資料の帰属情報 {#attribution-for-the-scrum-guide-expansion-pack-collection}

<!-- This collection was written and compiled by *Ralph Jocham, John Coleman, and Jeff Sutherland*. Each section is individually attributed above and retains its original license. The collection as a whole is for informational purposes; please respect the license terms of each section. -->

このコレクションは、_Ralph Jocham、John Coleman、Jeff Sutherland_ によって執筆・編纂された。各セクションは上記で個別に帰属が示されており、オリジナルのライセンスを保持している。コレクション全体は情報提供を目的としている。各セクションのライセンス条項を尊重して欲しい。

<!-- ## References -->

## 参考文献 {#references}

\[1\] Martin, R.L. (2022) A new way to think your guide to Superior Management Effectiveness. Boston, MA, MA, USA: Harvard Business Review Press.
\[2\] Gilb, T. & Graham, D. (1993) Software Inspection. Harlow: Addison-Wesley.
\[3\] Gilb, T. (1988) 'Deeper perspectives on evolutionary delivery, in Principles of Software Engineering Management. Wokingham: Addison-Wesley, pp. \[chapter 15\]. Also available at: [https://bit.ly/TomGilbEvo](https://bit.ly/TomGilbEvo).
\[4\] Gilb, Tom & Maier, Mark. (2005). Managing Priorities: A Key to Systematic Decision Making. INCOSE International Symposium. 15\. 10.1002/j.2334-5837.2005.tb00782.x. Also available at: [https://bit.ly/TomGilbPriorities](https://bit.ly/TomGilbPriorities).
\[5\] Gilb, T. (1988) 'Deeper perspectives on evolutionary delivery', in Principles of Software Engineering Management. Wokingham: Addison-Wesley, pp. \[chapter 15\].
\[6\] Gilb, T. (2005) Competitive Engineering: A Handbook for Systems Engineering, Requirements Engineering, and Software Engineering Using Planguage. Oxford: Elsevier Butterworth-Heinemann. Also available at: [https://bit.ly/TomGilbCompEng](https://bit.ly/TomGilbCompEng).
\[7\] Gilb, T. (2009) 'Agile specification quality control: Shifting emphasis from cleanup to sampling defects', Testing Experience, March. Available at: [https://www.researchgate.net/publication/294196272_Agile_specification_quality_control](https://www.researchgate.net/publication/294196272_Agile_specification_quality_control) \[Accessed: 17 May 2025\].
\[8\] Gilb, T. & Gilb, K. (1989) 'The McDonnell-Douglas case study of SQC and engineering improvement: Case DAC Inspection 1988–89'. Available at: [https://bit.ly/TomGilbMcDonnell-Douglas](https://bit.ly/TomGilbMcDonnell-Douglas) \[Accessed: 17 May 2025\].
\[9\] Blackburn, S. (2003) Ethics: A Very Short Introduction. Oxford: Oxford University Press.
\[10\] Frey, B.S. and Jegen, R. (2001) 'Motivation crowding theory', Journal of Economic Surveys, 15(5), pp. 589–611.
\[11\] Cameron, J., Banko, K.M. and Pierce, W.D. (2001) 'Pervasive negative effects of rewards on intrinsic motivation: The myth continues', The Behavior Analyst, 24(1), pp. 1–44.
\[12\] Deci, E.L., Koestner, R. and Ryan, R.M. (1999) 'A meta-analytic review of experiments examining the effects of extrinsic rewards on intrinsic motivation', Psychological Bulletin, 125(6), pp. 627–668.
\[13\] Ryan, R.M. and Deci, E.L. (2000) 'Intrinsic and extrinsic motivations: Classic definitions and new directions', Contemporary Educational Psychology, 25(1), pp. 54–67.
\[14\] Sandel, M.J. (2012) What money can't buy: The moral limits of markets. London: Allen Lane.
\[15\] Kohn, A. (1993) 'Why incentive plans cannot work', Harvard Business Review, 71(5), pp. 54–63.
\[16\] Scotland, K. (2023) Why strategy deployment? Here are three great reasons, AvailAgility. At: [https://availagility.co.uk/2023/02/16/why-strategy-deployment-here-are-three-great-reasons/](https://availagility.co.uk/2023/02/16/why-strategy-deployment-here-are-three-great-reasons/) (Accessed: April 3, 2023).
\[17\] Scotland, K. (2019) Deploying strategies as choices, AvailAgility. At: [https://availagility.co.uk/2019/02/08/deploying-strategies-as-choices/](https://availagility.co.uk/2019/02/08/deploying-strategies-as-choices/) (Accessed: April 3, 2023).
\[18\] Scotland, K. (2017) Strategy deployment and playing to win, AvailAgility. At: [https://availagility.co.uk/2017/07/14/strategy-deployment-and-playing-to-win/](https://availagility.co.uk/2017/07/14/strategy-deployment-and-playing-to-win/) (Accessed: April 3, 2023).
\[19\] Scotland, K. (2017) A strategy deployment cadence, AvailAgility. At: [https://availagility.co.uk/2017/09/06/a-strategy-deployment-cadence/](https://availagility.co.uk/2017/09/06/a-strategy-deployment-cadence/) (Accessed: April 3, 2023).
\[20\] Cagan, M. (2024) Transformed: Moving to the Product Operating Model. Hoboken, NJ: Wiley.
\[21\] Cagan, M. (2025) 'The Product Operating Model', Silicon Valley Product Group, 17 March. Available at: [https://www.svpg.com/the-product-operating-model/](https://www.svpg.com/the-product-operating-model/) (Accessed: 8 June 2025).
\[22\] Cagan, M. (n.d.) 'The Product Operating Model: An Introduction', Silicon Valley Product Group. Available at: [https://www.svpg.com/the-product-operating-model-an-introduction/](https://www.svpg.com/the-product-operating-model-an-introduction/) (Accessed: 8 June 2025\)
\[23\] Scrum.org (2025) 'The Agile Product Operating Model', Scrum.org, 1 May. Available at: [https://www.scrum.org/resources/agile-product-operating-model](https://www.scrum.org/resources/agile-product-operating-model) (Accessed: 8 June 2025).
\[24\] Scrum.org (2025) 'Agile Product Operating Model State of Play \- Part 1 \- Fundamentals', Scrum.org, 12 May. Available at: [https://www.scrum.org/resources/blog/agile-product-operating-model-state-play-part-1-fundamentals](https://www.scrum.org/resources/blog/agile-product-operating-model-state-play-part-1-fundamentals) (Accessed: 8 June 2025).
\[25\] Scrum.org (2024) 'Project to Product and the Agile Product Operating Model', Scrum.org, 7 November. Available at: [https://www.scrum.org/resources/blog/project-product-and-agile-product-operating-model](https://www.scrum.org/resources/blog/project-product-and-agile-product-operating-model) (Accessed: 8 June 2025).
\[26\] Scrum.org (2024) Moving to an Agile Product Operating Model \[PDF\]. Available at: [https://www.scrum.org/resources/moving-agile-product-operating-model-evidence-based-approach-delivering-products-digital-age](https://www.scrum.org/resources/moving-agile-product-operating-model-evidence-based-approach-delivering-products-digital-age) or [https://bit.ly/SDOAPOM](https://bit.ly/SDOAPOM). (Accessed: 8 June 2025\)
\[27\] Kniberg, H. and Ivarsson, A. (2012) Scaling at Spotify, Crisp. At: [https://blog.crisp.se/wp-content/uploads/2012/11/SpotifyScaling.pdf](https://blog.crisp.se/wp-content/uploads/2012/11/SpotifyScaling.pdf) (Accessed: April 5, 2023).
\[28\] Ambler, S.W. and Lines, M. (2023) Disciplined Agile® Toolkit \- Project Management Institute, PMI. At: [https://www.pmi.org/disciplined-agile/](https://www.pmi.org/disciplined-agile/) (Accessed: April 5, 2023).
\[29\] Leffingwell, D. and Knaster, R. (2023) Safe 6.0 framework, Scaled Agile Framework. At: [https://www.scaledagileframework.com/](https://www.scaledagileframework.com/) (Accessed: April 5, 2023).
\[30\] Sutherland, J. (2021) Scrum@Scale \- the scaling framework created by dr. Jeff Sutherland, Scrum@Scale Framework. At: [https://www.scrumatscale.com/](https://www.scrumatscale.com/) (Accessed: April 5, 2023).
\[31\] Skelton, M. and Pais, M. (2023) Team topologies, Team Topologies. At: [https://teamtopologies.com/](https://teamtopologies.com/) (Accessed: April 5, 2023).
\[32\] Appelo, J. (2023) Versatile Organization Design, unFIX. At: [https://unfix.com/](https://unfix.com/) (Accessed: April 5, 2023).
\[33\] Merel, P. (2023) Xscale Alliance, XSCALE Alliance. At: [https://xscalealliance.org/\#manifesto](https://xscalealliance.org/#manifesto) (Accessed: April 5, 2023).
\[34\] Schwaber, K. et al. (2021) Online nexus guide, Scrum.org. At: [https://www.scrum.org/resources/online-nexus-guide](https://www.scrum.org/resources/online-nexus-guide) (Accessed: April 5, 2023).
\[35\] Quartel, R. et al. (2024) FaST guide, Fluid Scaling Technology. At: [https://www.fastagile.io/](https://www.fastagile.io/) (Accessed: December 6, 2023).
\[36\] Ramos, C. and Pavlichenko, I. (2023) Creating agile organizations, Creating Agile Organizations. At: [https://creatingagileorganizations.com/](https://creatingagileorganizations.com/) (Accessed: April 15, 2023).
\[37\] Larman, C. & Vodde, B. (2025) LeSS (Large-Scale Scrum) Framework. Available at: [https://less.works/less/framework](https://less.works/less/framework) (Accessed: 8 June 2025\)
\[38\] Flight Levels GmbH (2025) Flight Levels Framework. Available at: [https://www.flightlevels.io/what-is-flight-levels/](https://www.flightlevels.io/what-is-flight-levels/) (Accessed: 8 June 2025).
\[39\] Krivitsky, A. and Flemm, R. (2022) Org topologies, Org Topologies. At: [https://www.orgtopologies.com/](https://www.orgtopologies.com/) (Accessed: April 4, 2023).
\[40\] Singh, P. (2023) Scaling Simplified: A Practitioner's Guide to Scaling Flow. Florida: Self-published. Available at: [https://leanpub.com/scalingsimplified](https://leanpub.com/scalingsimplified) (Accessed: 8 June 2025\)
\[41\] Scotland, K. (2022) The ultimate X-matrix for your agile transformation is here, AvailAgility. At: [https://availagility.co.uk/2022/11/03/the-ultimate-x-matrix-for-youragile-transformation-is-here/](https://availagility.co.uk/2022/11/03/the-ultimate-x-matrix-for-youragile-transformation-is-here/) (Accessed: April 5, 2023).
\[42\] Krebs, J. (2023) Agile kata pro, Agile Kata Pro. At: [https://agilekata.pro/](https://agilekata.pro/) (Accessed: April 4, 2023).
\[43\] Doerr, J. (2023) OKRs 101, What Matters. At: [https://www.whatmatters.com/get-started/](https://www.whatmatters.com/get-started/) (Accessed: April 4, 2023).
\[44\] Wodtke, C. (2021) Radical focus achieving your most important goals with objectives and key results--. Palo Alto, CA: Cucina Media.
\[45\] Gothelf, J. & Seiden, J. (2024) Who Does What By How Much?: A Practical Guide to Customer-Centric OKRs. New York: Sense & Respond Press.
\[46\] Appelo, J. (2023) Sometimes, you \*don't\* want focus, unFIX. At: [https://unfix.com/blog/sometimes-you-dont-want-focus](https://unfix.com/blog/sometimes-you-dont-want-focus) (Accessed: 14 January 2024).
\[47\] Appelo, J. (2023) Bets and objectives, unFIX. At: [https://unfix.com/bets-and-objectives](https://unfix.com/bets-and-objectives) (Accessed: 14 January 2024).
\[48\] McChesney, C. (2023) The 4 disciplines of execution (new), FranklinCovey. At: [https://www.franklincovey.com/the-4-disciplines/](https://www.franklincovey.com/the-4-disciplines/) (Accessed: April 4, 2023).
\[49\] Scrum.org (2024) Evidence-Based Management (EBM) Framework, Scrum.org. Available at: [https://www.scrum.org/resources/evidence-based-management](https://www.scrum.org/resources/evidence-based-management). (Accessed: 8 June 2025).
\[50\] Burrows, M. (2023) Home: Agendashift™, Agendashift. At: [https://www.agendashift.com/](https://www.agendashift.com/) (Accessed: April 4, 2023).
\[51\] [Cynefin.io](https://Cynefin.io/), V. (2022) Cynefin wiki, [Cynefin.io](https://Cynefin.io/). [Cynefin.io](https://Cynefin.io/). At: [https://cynefin.io/](https://cynefin.io/) (Accessed: April 4, 2023).
\[52\] Rancati, A. and Snowden, D. (2021) Managing complexity (and chaos) in a crisis \- a field guide for decision makers inspired by the Cynefin framework. Luxembourg, Belgium: Publications Office of the European Union.
\[53\] Snowden, D. et al. (2022) Cynefin® weaving sense-making into the fabric of our world. 2nd edn. Edited by R. Greenberg and B. Bertsch. Singapore, Singapore: Cognitive Edge \- The Cynefin Co.
\[54\] Snowden, D. (2023) Cynefin St David's 2023 1 of 2, Cynefin Co. [https://thecynefin.co/cynefin-st-davids-2023-1-of-2/](https://thecynefin.co/cynefin-st-davids-2023-1-of-2/) (Accessed: April 20, 2023).
\[55\] Snowden, D. (2023) Managing for emergence through abduction, The Cynefin Co. At: [https://thecynefin.co/managing-for-emergence/](https://thecynefin.co/managing-for-emergence/) (Accessed: June 24, 2023).
\[56\] Snowden, D. and Smith, N. (2023) Leadership discussion: Dave and Natalie \- the Cynefin co, YouTube. At: [https://youtu.be/WcPZ8ybDF0w](https://youtu.be/WcPZ8ybDF0w) (Accessed: April 7, 2023).
