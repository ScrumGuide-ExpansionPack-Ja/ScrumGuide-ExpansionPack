---
# title: Adaptive Enterprise (Expansion of the SGEP)
title: 適応力のある企業（SGEP拡張版）
# description: Adaptive enterprises are not built by choosing the right model, they are built by leaders who align words and actions and design decision-making close to the work.
description: 適応力のある企業は、適切なモデルを選ぶことで構築されるのではなく、言葉と行動を一致させ、仕事に近いところで意思決定を設計するリーダーによって構築される。
# keywords:
#   - Adaptive Enterprise
#   - Decentralised decision-making
#   - Say-do match
#   - Product Operating Model
keywords:
  - 適応力のある企業
  - 分散型意思決定
  - 言行一致
  - プロダクトオペレーティングモデル
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
  priority: 0.7
aliases:
  - /ja/adaptive-enterprise/2026.1/
---

<!-- ***Collected Resources for Scrum Guide Expansion Pack*** -->

**_スクラムガイド拡張パック収録資料_**

<!-- *This document is a collection of independent works. Each section retains its original license or copyright status, as indicated. Please refer to each section for specific usage rights and requirements.* -->

_本書は、独立した著作物を収録したものである。各セクションは記載の通り、オリジナルのライセンスや著作権状況を保持している。特定の使用権限と要件については、各セクションを参照して欲しい。_

<!-- License/Copyright: [CC BY-NC-ND 4.0](https://creativecommons.org/licenses/by-nc-nd/4.0/), © 2017-2025 Orderly Disruption Limited -->

ライセンス/著作権：[CC BY-NC-ND 4.0](https://creativecommons.org/licenses/by-nc-nd/4.0/)、© 2017-2025 Orderly Disruption Limited

<!-- Note: This section is included in its original, unaltered form with permission under the terms of the [CC BY-NC-ND 4.0](https://creativecommons.org/licenses/by-nc-nd/4.0/) license. No changes have been made. -->

注：このセクションは[CC BY-NC-ND 4.0](https://creativecommons.org/licenses/by-nc-nd/4.0/)ライセンスの条件に基づき、許可を得てオリジナルのまま変更なく収録されている。

---

<!-- It's difficult for an enterprise to be adaptive \[2\] without a climate where words and actions match. Over eighty engagement models were studied. Amongst those were scaling or descaling frameworks, and Product operating models, which can be useful for multi-Scrum-Team Products. Models range from going too far to not doing enough in helping the Product organization become more adaptive. There is no grand, universal truth or context-free 'Goldilocks zone.' -->

言葉と行動が一致する風土がなければ、適応力[2]のある企業であるのは困難である。80件以上のエンゲージメントモデルが研究された。その中には、複数スクラムチームのプロダクトに役立つスケーリング・デスケーリングのフレームワーク・プロダクトオペレーティングモデルが含まれる。これらのモデルには、適応力のあるプロダクト組織となる助けとして行き過ぎたものから全く不十分までさまざまなものがある。普遍的な真実や文脈を問わない「ゴルディロックスゾーン」は存在しない。

<!-- Of the engagement models studied, there are a number of notable contenders, including but not limited to Beyond Budgeting, Humanocracy, and Sociocracy, that, depending on the context, should be explored. Consider the combination with each other and with other approaches. -->

調査対象となったエンゲージメントモデルの中で注目すべき候補は多数存在する。脱予算経営、ヒューマノクラシー、ソシオクラシーを含むがこれに限定されない。文脈に応じてこれらを探求すべきである。相互に、あるいは他のアプローチと組み合わせて用いることを検討してほしい。

<!-- ## Beyond Budgeting -->

## 脱予算経営 {#beyond-budgeting}

<!-- Beyond Budgeting \[3-26\]is a management philosophy that rejects traditional, rigid annual budgeting in favor of a decentralized and adaptive approach to organizational control and performance management. It is built on 12 guiding principles-six focused on leadership and six on management processes-that promote decentralized decision-making, transparency, team autonomy, and a strong alignment with customer value. -->

脱予算経営[3-26]は、従来の硬直的な年次予算編成を否定し、分散型かつ適応的な組織管理・業績管理アプローチを取る経営哲学である。リーダーシップに関する6つの原則とマネジメントプロセスに関する6つの原則、計12の指針となる原則に基づいており、分散型の意思決定・透明性・チームの自律性・顧客価値との強い整合性を促進する。

<!-- Instead of fixed targets and detailed annual plans, Beyond Budgeting encourages dynamic goal-setting, continuous planning, and allocation informed by real-time needs, fostering adaptiveness and responsiveness in a rapidly changing business environment. This approach aims to empower teams, enhance innovation, and ensure organizations are better equipped to navigate uncertainty \[27\] and complexity \[28-33\]. Beyond Budgeting is badly named (false assumption it's only about Finance) and well named at the same time (indeed going beyond budgeting). -->

固定的な目標や詳細な年次計画の代わりに、脱予算経営は動的な目標設定・継続的計画・リアルタイムのニーズに基づく資源配分を奨励する。これにより、急速に変化するビジネス環境における適応性・反応性を高める。このアプローチは、チームのエンパワーメント・イノベーションの促進・不確実性[27]と複雑性[28-33]への組織対応力を高めることを目的としている。脱予算経営という名称は、財務にのみ焦点を当てているという誤解を生む不適切な名称と言える一方で、予算の枠を超えるという意味では適切な名称でもある。

<!-- ## Humanocracy -->

## ヒューマノクラシー {#humanocracy}

<!-- Humanocracy \[34\], as defined by Gary Hamel, is a management model that replaces rigid hierarchies and centralized control with systems that maximize each person's contribution and creativity. In a humanocracy, organizations exist to serve and empower people, not just treat employees as resources for company goals. -->

Gary Hamelにより提唱されたヒューマノクラシー[34]は、硬直的な階層構造や中央集権的な管理を廃し、個々人の貢献と創造性を最大限に引き出すシステムに置き換えるマネジメントモデルである。ヒューマノクラシーにおいて、組織は人々に奉仕し、力を与えるために存在するのであり、従業員を単なる企業目標達成のためのリソースとして扱うのではない。

<!-- It is built on principles like distributed ownership, meritocracy, openness, experimentation, and community, fostering autonomy and innovation. Authority is based on competence, and decision-making is decentralized to those closest to the work. Humanocracy prioritizes trust, engagement, and unleashing human potential over compliance and control, aiming to build resilient, innovative workplaces where employees drive meaningful change. -->

ヒューマノクラシーは、分散的なオーナーシップ・実力主義・公開性・実験・コミュニティといった原則に基づいており、自律性とイノベーションを育む。権限はコンピテンシーに基づいて与えられ、意思決定は現場に最も近い人々に分散される。ヒューマノクラシーは、コンプライアンスや統制よりも、信頼・エンゲージメント・人間の可能性の解放を優先し、レジリエンスと革新性に富んだ職場環境の構築を目指す。

<!-- While models like Haier's Rendanheyi \[35-36\]share values of decentralization and empowerment, humanocracy is a broader philosophy focused on replacing bureaucracy with people-centric principles that unlock collective capability and value. -->

ハイアール社の人単合一（RenDanHeYi）モデル[35-36]は分散化とエンパワーメントの価値を共有するが、ヒューマノクラシーは官僚主義を人間中心の原則に置き換え、集合的能力と価値を解き放つことを目的とするより広範な哲学である。

<!-- ## Sociocracy -->

## ソシオクラシー {#sociocracy}

<!-- Sociocracy \[37-41\] is a governance system that organizes people into self-managing \[42\] circles and makes decisions by consent, not majority vote. Developed by Gerard Endenburg \[43\] in the Netherlands in the 1970s, it ensures everyone affected by a decision has a voice, with proposals advancing unless a reasoned objection is raised. Guided by the principle of 'good enough for now, safe enough to try,' sociocracy distributes authority, promotes transparency, accountability, and continuous improvement, and fosters collaboration and shared ownership. Its principles have influenced models like Holacracy and self-managing teams. -->

ソシオクラシー[37-41]は、自己管理型[42]サークルに人々を組織し、多数決ではなく同意によって意思決定を行うガバナンスシステムである。1970年代にオランダのGerard Endenburg[43]によって開発され、意思決定の影響を受けるすべての人に発言権が与えられ、合理的な異議が提起されない限り提案が進む仕組みである。「今は十分、試すには十分安全」という原則に基づき、ソシオクラシーは権限の分散、透明性、説明責任、継続的改善、そしてコラボレーションとシェアード・オーナーシップを促進する。その原則はホラクラシーや自己管理チームなどのモデルに影響を与えている。

<!-- The most established variant is the Sociocratic Circle-Organization Method (SCM), the original, formalized method. SCM uses semi-autonomous circles, double-linking (where two people attend two directly related circles to connect those circles), consent-based decision-making, and open elections for roles. This structure maintains both organizational efficiency and member equivalence, and has a well-documented track record in businesses, cooperatives, and schools in the Netherlands. -->

最も確立された形式はSociocratic Circle-Organization Method（SCM）であり、これは元祖とも言える形式化された手法である。SCMでは、半自律的なサークル、ダブルリンク（2人が直接関連する2つのサークルに所属して接続する）、同意に基づく意思決定、そして役割の公開選挙が採用される。この構造は、組織の効率性とメンバーの対等性を維持し、オランダの企業、協同組合、学校において実績がある。

<!-- While newer variants like Sociocracy 3.0 (S3) offer more flexibility, SCM remains the most historically validated and widely documented form of sociocracy. -->

最近ではより柔軟性を高めているソシオクラシー 3.0（S3）のような新しいバリエーションもあるが、SCMは依然として最も歴史的に検証され、広く文書化されたソシオクラシーの形式である。

<!-- ## Attribution for the Scrum Guide Expansion Pack Collection -->

## スクラムガイド拡張パックにおける収録資料の帰属情報 {#attribution-for-the-scrum-guide-expansion-pack-collection}

<!-- This collection was written and compiled by *Ralph Jocham, John Coleman, and Jeff Sutherland*. Each section is individually attributed above and retains its original license. The collection as a whole is for informational purposes; please respect the license terms of each section. -->

このコレクションは、_Ralph Jocham、John Coleman、Jeff Sutherland_ によって執筆・編纂された。各セクションは上記で個別に帰属が示されており、オリジナルのライセンスを保持している。コレクション全体は情報提供を目的としている。各セクションのライセンス条項を尊重して欲しい。

<!-- ## References -->

## 参考文献 {#references}

\[1\] Coleman, J., (2025) MORE executive SUCCESS. Unpublished.
\[2\] LeSS (n.d.) 'Why LeSS? Achieving adaptiveness'. Available at: [https://less.works/less/framework/why-less](https://less.works/less/framework/why-less) (Accessed: 17 May 2025).
\[3\] Bogsnes, B. (2023) This is beyond budgeting: A guide to more adaptive and human organizations. Hoboken, NJ: John Wiley & Sons, Inc.
\[4\] Bogsnes, B. (2023) Beyond budgeting at 25 \- [bbrt.org](https://bbrt.org/), Beyond Budgeting Round Table. At: [https://bbrt.org/wp-content/uploads/bb-white-paper\_a.pdf](https://bbrt.org/wp-content/uploads/bb-white-paper_a.pdf) (Accessed: April 7, 2023).
\[5\] Olesen, A. (2016) Beyond budgeting: Principle 1 \- purpose, YouTube. At: [https://youtu.be/\_9ZW2NjyFxE](https://youtu.be/_9ZW2NjyFxE) (Accessed: April 7, 2023).
\[6\] Larsson, D. (2016) Beyond budgeting: Principle 2 \- values, YouTube. At: [https://youtu.be/pl1BPrITbm4](https://youtu.be/pl1BPrITbm4) (Accessed: April 7, 2023).
\[7\] Player, S. (2016) Beyond budgeting: Principle 3 \- transparency, YouTube. At: [https://youtu.be/Mb7K8App2vw](https://youtu.be/Mb7K8App2vw) (Accessed: April 7, 2023).
\[8\] Röösli, F. (2016) Beyond budgeting: Principle 4 \- Organization, YouTube. At: [https://youtu.be/i8HIgc8OZYM](https://youtu.be/i8HIgc8OZYM) (Accessed: April 7, 2023).
\[9\] Larsson, D. (2016) Beyond budgeting: Principle 5 \- autonomy, YouTube. At: [https://youtu.be/ipnjHtXYi-g](https://youtu.be/ipnjHtXYi-g) (Accessed: April 7, 2023).
\[10\] Player, S. (2016) Beyond budgeting: Principle 6 \- customers, YouTube. At: [https://youtu.be/\_6fut4R\_wVw](https://youtu.be/_6fut4R_wVw) (Accessed: April 7, 2023).
\[11\] Bogsnes, B. (2016) Beyond budgeting: Principle 7 \- rhythm, YouTube. At: [https://youtu.be/rb\_NsnPNIQQ](https://youtu.be/rb_NsnPNIQQ) (Accessed: April 7, 2023).
\[12\] Röösli, F. (2016) Beyond budgeting: Principle 8 \- targets, YouTube. At: [https://youtu.be/up3mp7jN6XU](https://youtu.be/up3mp7jN6XU) (Accessed: April 7, 2023).
\[13\] Player, S. (2016) Beyond budgeting: Principle 9 \- plans and forecasts, YouTube. At: [https://youtu.be/OWM7FUuXejI](https://youtu.be/OWM7FUuXejI) (Accessed: April 7, 2023).
\[14\] Olesen, A. (2016) Beyond budgeting: Principle 10 \- resource allocation, YouTube. At: [https://youtu.be/mPCYHmvi\_b8](https://youtu.be/mPCYHmvi_b8) (Accessed: April 7, 2023).
\[15\] Bogsnes, B. (2016) Beyond budgeting: Principle 11 \- performance evaluation, YouTube. At: [https://youtu.be/RfPVtG2B27E](https://youtu.be/RfPVtG2B27E) (Accessed: April 7, 2023).
\[16\] Röösli, F. (2016) Beyond budgeting: Principle 12 \- rewards, YouTube. At: [https://youtu.be/ETU5TzNYiC0](https://youtu.be/ETU5TzNYiC0) (Accessed: April 7, 2023).
\[17\] Morlidge, S. & Player, S., 2010\. Future Ready: How to Master Business Forecasting. Chichester: John Wiley & Sons.
\[18\] Morlidge, S., 2024\. The Little Book of Beyond Budgeting: A New Management Model for Organisations (Second Edition) \[Beyond Books Press\]
\[19\] Morlidge, S., 2019\. The Little (Illustrated) Book of Operational Forecasting. \[Troubador\].
\[20\] Morlidge, S., 2019\. Present Sense. \[Troubador\].
\[21\] Morlidge, S., 2021\. Zen and the Art of Organising Work. \[Troubador\].
\[22\] Morlidge, S., 2023\. Cost Matters. \[Beyond Books Press\].
\[23\] Beyond Budgeting i praktiken Fahlén, K., 2016\. Beyond Budgeting i praktiken. Stockholm: Liber.
\[24\] Fahlén, K., 2018\. Dynamic Management Strategy: A guide to management innovation and competitive advantage. Gothenburg: BAS
\[25\] Bogsnes, B., 2016\. Implementing Beyond Budgeting: Unlocking the Performance Potential. 2nd ed. Chichester: John Wiley & Sons.
\[26\] Becker, S et al (co-author) The Viable Map Workbook 2023 \[Beyond Books Press\]
\[27\] van der Bles, A.M., van der Linden, S., Freeman, A.L.J. and Spiegelhalter, D.J. (2019) 'Communicating uncertainty about facts, numbers and science', Royal Society Open Science, 6(5), 181870\. Available at: [https://www.ncbi.nlm.nih.gov/pmc/articles/PMC6549952/](https://www.ncbi.nlm.nih.gov/pmc/articles/PMC6549952/) (Accessed: 17 May 2025).
\[28\] [Cynefin.io](https://Cynefin.io/), V. (2022) Cynefin wiki, [Cynefin.io](https://Cynefin.io/). [Cynefin.io](https://Cynefin.io/). At: [https://cynefin.io/](https://cynefin.io/) (Accessed: April 4, 2023).
\[29\] Rancati, A. and Snowden, D. (2021) Managing complexity (and chaos) in a crisis \- a field guide for decision makers inspired by the Cynefin framework. Luxembourg, Belgium: Publications Office of the European Union.
\[30\] Snowden, D. et al. (2022) Cynefin® weaving sense-making into the fabric of our world. 2nd edn. Edited by R. Greenberg and B. Bertsch. Singapore, Singapore: Cognitive Edge \- The Cynefin Co.
\[31\] Snowden, D. (2023) Cynefin St David's 2023 1 of 2, Cynefin Co. [https://thecynefin.co/cynefin-st-davids-2023-1-of-2/](https://thecynefin.co/cynefin-st-davids-2023-1-of-2/) (Accessed: April 20, 2023).
\[32\] Snowden, D. (2023) Managing for emergence through abduction, The Cynefin Co. At: [https://thecynefin.co/managing-for-emergence/](https://thecynefin.co/managing-for-emergence/) (Accessed: June 24, 2023).
\[33\] Snowden, D. and Smith, N. (2023) Leadership discussion: Dave and Natalie \- the Cynefin co, YouTube. At: [https://youtu.be/WcPZ8ybDF0w](https://youtu.be/WcPZ8ybDF0w) (Accessed: April 7, 2023).
\[34\] Hamel, G. and Zanini, M. (2023) Humanocracy. At: [https://www.humanocracy.com/](https://www.humanocracy.com/) (Accessed: April 5, 2023).
\[35\] Fischer, B., Minnaar, J., Moehrle, M., & Cornuel, E. (2020) RenDanHeYi: Pioneering the Quantum Organisation. EFMD Global Focus, Special Supplement. Available at: [https://bit.ly/RenDanHeYi](https://bit.ly/RenDanHeYi) \[Accessed 27 May 2025\]
\[36\] Williamson, P.J. & Yin, E. (2018) 'Management Innovation Made in China: Haier's Rendanheyi', California Management Review, 61(1), pp. 71-93.
\[37\] Rau, T. (2022) Sociocracy \- Basic Concepts and principles, Sociocracy For All. At: [https://www.sociocracyforall.org/sociocracy/](https://www.sociocracyforall.org/sociocracy/) (Accessed: April 5, 2023).
\[38\] Buck, J. & Endenburg, G. (2012) The creative forces of self-organization. Sociocratic Center.
\[39\] Buck, J. & Villines, S. (2017) We the people: Consenting to a deeper democracy. 2nd edn. Sociocracy.info Press.
\[40\] Endenburg, G. (1998) Sociocracy: The organization of decision-making. Delft: Eburon Publishers.
\[41\] Priest, J. & Bockelbrink, B. (2018) Sociocracy 3.0 – The practical guide. Available at: [https://sociocracy30.org/](https://sociocracy30.org/) (Accessed: 17 May 2025).
\[42\] LeSS.works (n.d.) Self-managing teams. Available at: [https://less.works/less/management/self-managing-teams](https://less.works/less/management/self-managing-teams) (Accessed: 17 May 2025).
\[43\] Sociocracy For All (n.d.) 'Gerard Endenburg: founder of Sociocratic Circle Method and pioneer of self-management'. Available at: [https://www.sociocracyforall.org/gerard-endenburg-founder-of-sociocratic-circle-method-and-pioneer-of-self-management/](https://www.sociocracyforall.org/gerard-endenburg-founder-of-sociocratic-circle-method-and-pioneer-of-self-management/) (Accessed: 18 May 2025).
