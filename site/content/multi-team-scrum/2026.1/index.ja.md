---
# title: Multi Team Scrum (Expansion of the SGEP)
title: 複数チームスクラム（SGEP拡張版）
# description: Guidance for leaders and practitioners deciding whether and how to scale Scrum, showing when multiple teams on one Product increase outcomes and when they simply add coordination overhead.
description: スクラムをスケーリングするかどうか、またどのようにスケーリングするかを決定するリーダーや実践者へのガイダンス。複数チームが1つのプロダクトに取り組むことでアウトカムが増加する場合と、単に調整のオーバーヘッドが増加するだけの場合を示す。
# keywords:
#   - Mutli-Team Scrum
#   - Aligned autonomy
#   - Shared Product Backlog
#   - Continuous Integration
keywords:
  - 複数チームスクラム
  - 調整された自律性
  - 共有プロダクトバックログ
  - 継続的インテグレーション
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
forked_from: scrum-guide-expansion-pack/2025.6
sitemap:
  priority: 0.7
aliases:
  - /ja/multi-team-scrum/2026.1/
---

<!-- **_Collected Resources for Scrum Guide Expansion Pack_** -->

**_スクラムガイド拡張パック収録資料_**

<!-- _This document is a collection of independent works. Each section retains its original license or copyright status, as indicated. Please refer to each section for specific usage rights and requirements._ -->

_本書は、独立した著作物を収録したものである。各セクションは記載の通り、オリジナルのライセンスや著作権状況を保持している。特定の使用権限と要件については、各セクションを参照して欲しい。_

<!-- _License: Creative Commons Attribution-ShareAlike 4.0 International ([CC BY-SA 4.0](https://creativecommons.org/licenses/by-sa/4.0/))._ -->

_ライセンス：クリエイティブ・コモンズ 表示-継承 4.0 国際（[CC BY-SA 4.0](https://creativecommons.org/licenses/by-sa/4.0/)）_

<!-- © _2025 Ralph Jocham, John Coleman, and Jeff Sutherland._ -->

© _2025 Ralph Jocham、John Coleman、Jeff Sutherland_

<!-- _Disclaimer: No warranties are given. Use at your own risk._ -->

_免責事項：いかなる保証も提供されない。各自の責任で利用して欲しい。_

<!-- _This section is offered under the Attribution-ShareAlike 4.0 International license of Creative Commons._ -->

_このセクションは、クリエイティブ・コモンズの表示-継承4.0国際ライセンスの下で提供されている。_

<!-- _By using this Scrum Guide Expansion Pack, you agree to the terms of the [CC BY-SA 4.0](https://creativecommons.org/licenses/by-sa/4.0/) license._ -->

_このスクラムガイド拡張パックを使用することで、[CC BY-SA 4.0](https://creativecommons.org/licenses/by-sa/4.0/)ライセンスの条項に同意したものとみなされる。_

---

<!-- If a Scrum Team becomes too large, it should consider reorganizing into multiple cohesive Scrum Teams, each focused on the same Product. Multiple Scrum Teams on the same Product should share the same Product Goal, Product Backlog, Product Owner, baseline Definition of Outcome Done, and baseline Definition of Output Done. -->

スクラムチームが大きくなりすぎた場合、同じプロダクトに集中する、複数の結束したスクラムチームに再編成することを検討すべきである。同じプロダクトに複数のスクラムチームが存在する場合、それらのチームは共通のプロダクトゴール、プロダクトバックログ、プロダクトオーナー、基準となるアウトカム完成の定義およびアウトプット完成の定義を共有する必要がある。

<!-- Be careful with blind assumptions that more value is produced from more Scrum Teams. Scale only when the benefits clearly outweigh the additional overhead. Before you scale, the single Scrum Team setup has to be able to reliably produce an Increment every Sprint. But if you must scale, use an approach that is coherent with this document. Often, fewer teams result in more outcomes. -->

スクラムチームの数が増えればより多くの価値が生み出されるという盲目的な思い込みには注意が必要である。スケーリングを行うのは、追加される負荷を上回る明確な利点がある場合に限る。スケーリングを行う前に、単一のスクラムチームが毎スプリント確実にインクリメントを提供できる状態にあることが必要である。スケーリングが避けられない場合には、本書の内容と整合性のあるアプローチを使用するとよい。多くの場合、チームが少ない方がより多くのアウトカムを生み出す。

<!-- In a multi-Scrum-Team context, Scrum Teams may reduce inter-Scrum-Team dependencies by becoming more cross-functional through collaboration, cross-pollination, transfer of learning, and intentional interactions. The specific skills needed are often broad and will vary with the domain of work. In a multi-Scrum-Team setting, purposeful and intentional interactions and professionalism (including continuous integration) become even more important. -->

複数のスクラムチームの文脈においては、コラボレーション、他家受粉、学習の移転、意図的な相互作用を通じて、より機能横断になることでチーム間の依存関係を減らすことができる。必要なスキルは多岐にわたることが多く、業務領域によって異なる。こうした状況下では、意図的で目的のある相互作用やプロフェッショナリズム（継続的インテグレーションを含む）が一層重要となる。

<!-- In a one Product Owner and one Scrum Team setup, the Product Owner could be a Product manager, marketing director, technology director, etc. In a multi-Scrum-Team setup for a Product, the ideal is still only one Product Owner, who should be a leader for the Product. To allow the Product Owner to handle multiple Scrum Teams on the same Product, the Product Owner often becomes more strategic and delegates problems to solve and opportunities to the Product Developers, including, for example, aspects of Product design or Product management. -->

1人のプロダクトオーナーと1つのスクラムチームという構成では、プロダクトオーナーはプロダクトマネージャー、マーケティングディレクター、技術部門責任者などを担うこともある。プロダクトに対して複数のスクラムチームが存在する構成では、理想としては依然としてプロダクトオーナーは1人のみであり、プロダクトに対するリーダーであるべきである。複数のスクラムチームに対応するため、プロダクトオーナーはより戦略的な役割を担い、問題の解決や機会の実現をプロダクト開発者に委任することが多くなる。たとえば、プロダクトの設計やプロダクトマネジメントの側面などが該当する。

<!-- The Product Backlog is a tool for increasing transparency. -->

プロダクトバックログは透明性を高めるためのツールである。

<!-- Generally, the fewer Product Backlogs per Product, implicit (like a filter of a Product Backlog) or explicit: -->

一般的に、暗黙的（プロダクトバックログのフィルターのように）にしろ明示的にしろ、プロダクトあたりのプロダクトバックログが少ないほど良い：

<!-- - The fewer the silos in the Product and the greater the transparency across the entire Product; -->
<!-- - The more transparent the overall progress tracking across the entire Product; -->
<!-- - The better the big-picture value clarity across the entire Product; -->
<!-- - The more likely a Scrum Team would know it's working on low-value items from a Product perspective; -->
<!-- - The more likely one is to observe improvement in the attainment of value; and, -->
<!-- - The more strategic the Product Owner becomes by delegating cross-Product work to the Product Developers. -->

- プロダクト内のサイロが減少し、プロダクト全体の透明性が高まる。
- プロダクト全体における進捗の追跡がより透明になる。
- プロダクト全体のビッグピクチャーとしての価値の明確さが増す。
- スクラムチームがプロダクトの観点から低い価値のアイテムに取り組んでいることに気づきやすくなる。
- 価値の達成における改善が見られやすくなる。
- プロダクトオーナーは、プロダクトを横断する作業をプロダクト開発者に委任することで、より戦略的な役割を担うようになる。

<!-- Fewer Product Backlogs per Product are better for adaptiveness \[1\], but without empowered ownership, a coherent span of control, or direct contact with relevant Stakeholders, gaps will arise. Scrum fosters a climate for happenstance and multi-learning as various people and Scrum Teams collaborate, discoveries and insights can be shared and leveraged. This is unlikely to happen in an environment where each component has a Product Backlog in isolation. -->

プロダクトあたりのプロダクトバックログが少ないほど、適応性[1]は高まる。しかし、権限委譲されたオーナーシップ、整合性のある管理範囲、または関連するステークホルダーとの直接的な接点がない場合には、ギャップが生じる。スクラムにより様々な人々やスクラムチームがコラボレーションし、発見や洞察が共有され活用されるように、スクラムは偶発性と多重学習のための土壌を育む。これは、各コンポーネントが孤立したプロダクトバックログを持つ環境では起こりにくい。

<!-- Happenstance in the context of 'The New New Product Development Game' \[2\] means that sometimes useful ideas or solutions come about by chance, not by careful planning. When Scrum Teams work closely together and share information, they might discover new approaches or answers simply because they are open to unexpected events or accidental findings. -->

「The New New Product Development Game」[2]の文脈における偶然性とは、有用なアイデアや解決策が、綿密な計画ではなく偶然によって生まれることを意味する。スクラムチームが密接に連携し、情報を共有していると、予期せぬ出来事や偶然の発見によって新しいアプローチや答えを見出すことがある。

<!-- Multi-learning means that team members learn in many different ways at the same time. They pick up new skills and knowledge not only in their own area but also in other areas, and they learn as individuals, as a group, and as part of the whole company. This helps the team become more flexible and able to solve a wide range of problems quickly, because everyone is learning from each other and from their experiences as they work together. -->

マルチラーニングとは、チームメンバーが同時に様々な方法で学習することを意味する。メンバーは自分の専門領域だけでなく、他の分野においてもスキルや知識を習得し、個人として、グループとして、そして会社全体の一員として学習していく。これにより、チームは柔軟性を持ち、幅広い課題を迅速に解決できるようになる。なぜなら、全員が互いから学び、共に働く中での経験から学び続けているからである。

<!-- Finding the right balance is a dilemma. There are always trade-offs to consider. However, a good heuristic is: The fewer Product Backlogs, implicit or explicit, the better, enabled through multi-learning and the organizational transfer of learning across Scrum Teams, departments, and Products. -->

適切なバランスを見つけることはジレンマである。常に考慮すべきトレードオフがある。しかし、良い経験則として、プロダクトごとのプロダクトバックログは暗黙的か明示的かを問わず少ない方が良い。それは、マルチラーニングとスクラムチーム、部門、プロダクトを横断した組織的な学習の移転によって実現される。

<!-- Organizational transfer of learning, as described in 'The New New Product Development Game' \[2\], is the process by which knowledge and insights gained in one new Product development area are regularly shared and applied to subsequent areas or other divisions within the organization. -->

「The New New Product Development Game」[2]で説明されている組織的な学習の移転とは、ある新製品開発の領域で得られた知識や洞察が、後続の領域や他の部門にも継続的に共有され適用されるプロセスを指す。

<!-- Organizations are often designed for ease of management over ease of outcomes. Ask yourself how many Scrum Teams a problem or opportunity touches to deliver value; generally, the lower that number, the better. -->

組織は往々にして、成果を出すための容易さよりも、管理するための容易さを優先して設計される。価値を届けるために、いくつのスクラムチームがその課題や機会に関与するかを自問してみてほしい。一般的には、その数が少ないほど良い。

<!-- Free teams from command and control. Err on the side of aligned autonomy. Foster purposeful, intentional interactions within and between self-managing Scrum Teams \[3\]. Foster a work climate with minimal but sufficient management processes, scaffolding, and boundaries. Balance and nurture Stakeholder expectations and limits. Build change agency and continual improvement in a direction, not just delivery, into a cadence. -->

チームを指揮統制から解き放つ。調整された自律性を重視する。自己管理スクラムチーム[3]の中およびその間で、目的のある意図的な相互作用を育む。最小限でありながら十分なマネジメントのプロセス、足場、境界のある働く環境を醸成する。ステークホルダーの期待と制約のバランスをとり、育成する。単なるデリバリーではなく、方向性のある変革推進力と継続的改善をケイデンスの中に組み込む。

<!-- When in doubt, study the New New Product Development Game \[2\], embrace the good of what's new in the present, but abandon any notions of an industrial complex \[4-9\] where only the brave people have the agency to do anything. -->

判断に迷ったときには「The New New Product Development Game」[2]を研究し、現代における新しいものの良さを受け入れつつ、勇敢な人だけが行動力を持つような産業複合体[4-9]の思考は捨てるべきである。

<!-- ## Attribution for the Scrum Guide Expansion Pack Collection -->

## スクラムガイド拡張パックにおける収録資料の帰属情報 {#attribution-for-the-scrum-guide-expansion-pack-collection}

<!-- This collection was written and compiled by _Ralph Jocham, John Coleman, and Jeff Sutherland_. Each section is individually attributed above and retains its original license. The collection as a whole is for informational purposes; please respect the license terms of each section. -->

このコレクションは、_Ralph Jocham、John Coleman、Jeff Sutherland_ によって執筆・編纂された。各セクションは上記で個別に帰属が示されており、オリジナルのライセンスを保持している。コレクション全体は情報提供を目的としている。各セクションのライセンス条項を尊重して欲しい。

<!-- ## References -->

## 参考文献 {#references}

\[1\] LeSS (n.d.) 'Why LeSS? Achieving adaptiveness'. Available at: [https://less.works/less/framework/why-less](https://less.works/less/framework/why-less) (Accessed: 17 May 2025).

\[2\] Takeuchi, H. and Nonaka, I. (2014) The new new product development game, Harvard Business Review. At: [https://hbr.org/1986/01/the-new-new-product-development-game](https://hbr.org/1986/01/the-new-new-product-development-game) (Accessed: 21 January 2024).

\[3\] LeSS.works (n.d.) Self-managing teams. Available at: [https://less.works/less/management/self-managing-teams](https://less.works/less/management/self-managing-teams) (Accessed: 17 May 2025).

\[4\] [Cynefin.io](https://Cynefin.io/), V. (2022) Cynefin wiki, [Cynefin.io](https://Cynefin.io/). [Cynefin.io](https://Cynefin.io/). At: [https://cynefin.io/](https://cynefin.io/) (Accessed: April 4, 2023).

\[5\] Rancati, A. and Snowden, D. (2021) Managing complexity (and chaos) in a crisis \- a field guide for decision makers inspired by the Cynefin framework. Luxembourg, Belgium: Publications Office of the European Union.

\[6\] Snowden, D. et al. (2022) Cynefin® weaving sense-making into the fabric of our world. 2nd edn. Edited by R. Greenberg and B. Bertsch. Singapore, Singapore: Cognitive Edge \- The Cynefin Co.

\[7\] Snowden, D. (2023) Cynefin St David's 2023 1 of 2, Cynefin Co. [https://thecynefin.co/cynefin-st-davids-2023-1-of-2/](https://thecynefin.co/cynefin-st-davids-2023-1-of-2/) (Accessed: April 20, 2023).

\[8\] Snowden, D. (2023) Managing for emergence through abduction, The Cynefin Co. At: [https://thecynefin.co/managing-for-emergence/](https://thecynefin.co/managing-for-emergence/) (Accessed: June 24, 2023).

\[9\] Snowden, D. and Smith, N. (2023) Leadership discussion: Dave and Natalie \- the Cynefin co, YouTube. At: [https://youtu.be/WcPZ8ybDF0w](https://youtu.be/WcPZ8ybDF0w) (Accessed: April 7, 2023).
