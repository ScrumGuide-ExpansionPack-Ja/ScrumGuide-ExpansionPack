---
# title: Scrum on One Page (Expansion of the SGEP)
title: スクラム1ページ要約（SGEP拡張版）
# description: Scrum on one page, expanded for modern product work. A concise, practical view of Scrum's roles, events, and commitments, with added clarity for complexity, product thinking, and evidence-based delivery.
description: 現代のプロダクト作業向けに拡張されたスクラム1ページ要約。スクラムの役割、イベント、コミットメントを簡潔かつ実践的に示し、複雑性、プロダクト思考、エビデンスに基づくデリバリーについて明確にする。
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
  priority: 0.7
aliases:
  - /ja/scrum-on-one-page/2026.1/
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

<!-- Scrum is described in the [2020 Scrum Guide](https://scrumguides.org/) (40). Scrum is a lightweight framework for addressing complex (30-35) work, particularly in Product discovery, development, delivery, and value realization. Scrum is based on empirical process control (decisions informed by evidence) and lean thinking (reducing waste and focusing on the flow of value) (63). Scrum is purposefully incomplete, guiding interactions rather than prescribing detailed recipes. -->

スクラムは、[2020年版スクラムガイド](https://scrumguides.org/)(40)で説明されている。スクラムは複雑(30-35)な作業、特にプロダクトの発見・開発・提供・価値実現に対応するための軽量なフレームワークである。スクラムは経験的プロセス制御（エビデンスに基づく意思決定）およびリーン思考（ムダを減らし価値の流れに集中する）に基づいている(63)。スクラムは意図的に不完全であり、詳細な手順を規定するのではなく、相互作用を導くものである。

<!-- **Why Use Scrum?** -->

**なぜスクラムを使うのか？**

<!-- Scrum enables Scrum Teams to identify, represent, or measure emergence (71), embrace uncertainty, respond to change, deliver and validate value frequently, and continuously improve. Scrum fosters collaboration, accountability, and evidence-informed decision-making, fostering the best possible outcomes in a rapidly changing environment. Self-managing Scrum Teams, organized around value, are crucial for creative problem-solving and opportunity capture; non-self-managing Scrum Teams hinder the ability to deal with complexity (30-35). Self-managing Scrum Teams are not to be confused with individual self-management. -->

スクラムは、スクラムチームが創発(71)を識別・表現・評価し、不確実性を受け入れ、変化に対応し、頻繁に価値を提供・検証し、継続的に改善することを可能にする。スクラムは、コラボレーション・説明責任・エビデンスに基づく意思決定を促進し、急速に変化する環境において最良のアウトカムを生み出す。価値を中心に組織された自己管理スクラムチームは、創造的な問題解決や機会の獲得において重要である。自己管理されていないスクラムチームは、複雑性(30-35)に対処する能力を妨げる。自己管理スクラムチームは、個人の自己管理と混同すべきではない。

<!-- **Elements of Scrum** -->

**スクラムの要素**

<!-- 1\. Scrum Theory: Built on three pillars: -->

1\. スクラムの理論：三本柱に基づく

<!-- - Transparency – Making work and value visible for Inspection. -->
<!-- - Inspection – Regularly assessing progress and outcomes for Adaptation. -->
<!-- - Adaptation – Adjusting plans informed by insights and feedback. -->

- 透明性：検査のために作業と価値を可視化する。
- 検査：適応のために進捗とアウトカムを定期的に評価する。
- 適応：洞察とフィードバックに基づいて計画を調整する。

<!-- 2\. Scrum Values: -->

2\. スクラムの価値基準：

<!-- - _Focus_, _Openness_, _Courage_, _Commitment_, and _Respect_ enable effective teamwork; they support trust. -->

- _集中_、_公開_、_勇気_、_確約_、_尊敬_ は効果的なチームワークを可能にし、信頼を築く。

<!-- 3\. _Roles_ / Accountabilities: -->

3\. _役割_ / 説明責任：

<!-- - Scrum Team – A small, self-managing, cross-functional, cognitively diverse team consisting of: -->
<!--   - Product Owner – Maximizes long-term value, engages Stakeholders, and manages the Product Backlog. -->
<!--   - Scrum Master – Guides the Scrum adoption, removes impediments, and fosters continuous improvement. -->
<!--   - Product Developers – Deliver Increments every Sprint through their cross-functional capabilities. -->
<!-- - _Stakeholder \- an entity, individual, or group interested in, affected by, or impacting inputs, activities, and outcomes with a direct or indirect interest inside or outside the organization, its Products, or services._ -->
<!--   - _Supporter, a Stakeholder type – Fosters the climate and environment and participates as requested._ -->
<!--   - _AI – As a tool or also a possible Product Developer, but not to be entirely trusted yet._ -->

- スクラムチーム：小さく、自己管理され、機能横断型で、認知的多様性を持ったチームであり、以下で構成される：
  - プロダクトオーナー：長期的な価値を最大化し、ステークホルダーを巻き込み、プロダクトバックログを管理する。
  - スクラムマスター：スクラム適用を導き、障害物を除去し、継続的改善を促進する。
  - プロダクト開発者：機能横断型スキルを通じてスプリントごとにインクリメントをデリバリーする。
- _ステークホルダー：組織・プロダクト・サービスの内外に直接的・間接的な利害関係を持ち、インプット・活動・アウトカムに関心を持ち、影響を受け・影響を与える個人・団体・グループ。_
  - _サポーター（ステークホルダーの一種）：風土と環境を育み、要請に応じて参加する。_
  - _AI：ツールとして、あるいはプロダクト開発者となる可能性もあるが、まだ完全に信頼すべきではない。_

<!-- 4\. Scrum Events & Activities -->

4\. スクラムイベント & 活動

<!-- - Scrum operates in Sprints (iterations of determinate length _up to four weeks_) with four timeboxed events: -->
<!-- - Sprint Planning – Define the Sprint Goal and plan the work. -->
<!-- - Daily Scrum – Product Developers align daily on progress toward the Sprint Goal or Product Goal. -->
<!-- - Sprint Review – Inspect the Increment, value, and marketplace, and adapt the Product Backlog. -->
<!-- - Sprint Retrospective – Reflect and improve the Scrum Team. -->
<!-- - Refinement – Clarify upcoming or selected work, formally (_as an optional event_) or informally -->

- スクラムはスプリント（_最長4週間_ の決められた期間のイテレーション）で運用され、4つのタイムボックス化されたイベントがある：
- スプリントプランニング：スプリントゴールを定義し、作業計画を立てる。
- デイリースクラム：プロダクト開発者が日々、スプリントゴールまたはプロダクトゴールに向けた進捗を調整する。
- スプリントレビュー：インクリメント、価値、市場を検査し、プロダクトバックログを適応させる。
- スプリントレトロスペクティブ：スクラムチームとして振り返り、改善する。
- リファインメント：正式に（_必須でないイベントとして_）または非公式に、今後の作業または選択された作業を明確にする。

<!-- 5\. Scrum Artifacts & Commitments -->

5\. スクラムの作成物 & コミットメント

<!-- - _Product & Definition of Outcome Done – Product and valuable outcomes that provide evidence of realized benefits._ -->
<!-- - Increment & Definition of Output Done – A potentially valuable, releasable candidate update for the Product. -->
<!-- - Product Backlog & Product Goal – the ordered (sequenced) list of work to achieve a medium-term, more strategic objective. -->
<!-- - Sprint Backlog & Sprint Goal – Selected Product Backlog Items and a plan for the Sprint, short-term objective. -->

- _プロダクト & アウトカム完成の定義：実現した利益のエビデンスとなるプロダクトおよび価値のあるアウトカム。_
- インクリメント & アウトプット完成の定義：潜在的に価値があり、リリース可能なプロダクトのリリース候補アップデート。
- プロダクトバックログ & プロダクトゴール：中期的でより戦略的な目標を達成するため、（一列に）順序付けされた作業リスト。
- スプリントバックログ & スプリントゴール：選択されたプロダクトバックログアイテムと、スプリントの短期的な目標に向けた計画。

<!-- ## Attribution for the Scrum Guide Expansion Pack Collection {#attribution-for-the-scrum-guide-expansion-pack-collection} -->

## スクラムガイド拡張パックにおける収録資料の帰属情報 {#attribution-for-the-scrum-guide-expansion-pack-collection}

<!-- This collection was written and compiled by _Ralph Jocham, John Coleman, and Jeff Sutherland_. Each section is individually attributed above and retains its original license. The collection as a whole is for informational purposes; please respect the license terms of each section. -->

このコレクションは、_Ralph Jocham、John Coleman、Jeff Sutherland_ によって執筆・編纂された。各セクションは上記で個別に帰属が示されており、オリジナルのライセンスを保持している。コレクション全体は情報提供を目的としている。各セクションのライセンス条項を尊重して欲しい。
