---
# title: Holistic Testing, Quality Engineering, and Scrum (Expansion of the SGEP)
title: ホリスティックテスティング、品質エンジニアリング、そしてスクラム（SGEP拡張版）
# description: Holistic Testing explains how Scrum Teams build quality in from discovery to production, using fast feedback, small changes, automation, observability, and safe releases to reduce risk and deliver customer value.
description: ホリスティックテスティングは、スクラムチームが発見からプロダクションまで品質を作り込む方法を説明する。迅速なフィードバック、小さな変更、自動化、オブザーバビリティ、安全なリリースを活用してリスクを低減し、顧客価値を提供する。
# keywords:
#   - Holistic Testing
#   - Built-in quality
#   - Fast feedback loops
#   - Whole-Team responsibility
keywords:
  - ホリスティックテスティング
  - 品質の作り込み
  - 迅速なフィードバックループ
  - チーム全体の責任
author:
  - Lisa Crispin
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
sitemap:
  priority: 0.7
aliases:
  - /ja/holistic-testing/2026.1/
---

<!-- **_Collected Resources for Scrum Guide Expansion Pack_** -->

**_スクラムガイド拡張パック 収録資料集_**

<!-- _This document is a collection of independent works. Each section retains its original license or copyright status, as indicated. Please refer to each section for specific usage rights and requirements._ -->

_この文書は独立した著作物のコレクションである。各セクションは示されているとおり、元のライセンスまたは著作権の状態を保持している。具体的な使用権と要件については、各セクションを参照してほしい。_

<!-- License/Copyright: [CC BY-NC-ND 4.0](https://creativecommons.org/licenses/by-nc-nd/4.0/) -->

ライセンス/著作権: [CC BY-NC-ND 4.0](https://creativecommons.org/licenses/by-nc-nd/4.0/)

<!-- Note: This section is included in its original, unaltered form with permission under the terms of the [CC BY-NC-ND 4.0](https://creativecommons.org/licenses/by-nc-nd/4.0/) license. No changes have been made. -->

注: このセクションは、[CC BY-NC-ND 4.0](https://creativecommons.org/licenses/by-nc-nd/4.0/) ライセンスの条項に基づき、許可を得て元の形式のまま収録されている。変更は加えられていない。

---

<!-- Cross-functional Scrum Teams collaborate closely with customers, users, Stakeholders, and Supporters to deliver products that their customers value. The Supporters and customers expect quality to be built into the products. The entire Scrum Team is responsible for quality and testing. Testing activities occur throughout the whole infinite loop of software development. -->

機能横断型のスクラムチームは、顧客、ユーザー、ステークホルダー、サポーターと緊密に協力して、顧客が価値を認めるプロダクトを提供する。サポーターと顧客は、品質がプロダクトに作り込まれていることを期待する。スクラムチーム全体が品質とテストに責任を持つ。テスト活動は、ソフトウェア開発の無限ループ全体を通じて行われる。

<!-- Consider testing from a holistic point of view. There are so many types of testing activities. The Holistic Testing Model provides a visual thinking tool to help Scrum Teams plan a comprehensive testing strategy that includes the entire development life cycle. Quality engineers, known by a variety of other job titles, are, as Product Developers, part of the Scrum Team and partner with the Product Owner and operations to embed quality throughout the life cycle. -->

ホリスティック（全体論的）な視点からテストを考えよう。テスト活動には非常に多くの種類がある。ホリスティックテスティングモデルは、スクラムチームが開発ライフサイクル全体を含む包括的なテスト戦略を計画するのに役立つ視覚的思考ツールを提供する。さまざまな役職名で知られる品質エンジニアは、プロダクト開発者としてスクラムチームの一員であり、プロダクトオーナーや運用担当者と連携してライフサイクル全体を通じて品質を組み込む。

<!-- ## **The Holistic Testing Model** -->

## ホリスティックテスティングモデル {#the-holistic-testing-model}

<!-- The Holistic Testing Model reflects the need for the whole Scrum Team to take ownership of quality and testing, engaging in testing activities around the whole infinite loop of software development. On the left side of the loop, these activities aim to prevent problems by identifying risks, prioritizing quality attributes [1][2] (also referred to as non-functional requirements, or NFRs) such as security and performance, surfacing hidden assumptions, and including all necessary capabilities. Testing extends around the right side of the loop, in both pre-production and production environments. -->

ホリスティックテスティングモデルは、スクラムチーム全体が品質とテストのオーナーシップを持ち、ソフトウェア開発の無限ループ全体を通じてテスト活動に従事する必要性を反映している。ループの左側では、これらの活動はリスクの特定、セキュリティやパフォーマンスなどの品質特性 [1][2]（非機能要件またはNFRとも呼ばれる）の優先順位付け、隠れた前提の表面化、必要なすべての機能の組み込みによって問題を予防することを目的としている。テストはループの右側、プリプロダクション環境とプロダクション環境の両方に広がる。

<!-- There are no handoffs between Scrum Teams in modern software testing. The pauses in the model indicate a time for the Scrum Team to pause and reflect on what they've done so far and whether they are ready to continue to the next stage. There are no rules about how long the Scrum Team should spend in each stage when implementing a new change to a product. They may get to a stage and realize they have to circle back to a previous stage where they missed something. -->

現代のソフトウェアテストでは、スクラムチーム間の引き継ぎは存在しない。モデル内の一時停止は、スクラムチームがこれまでの作業を振り返り、次のステージに進む準備ができているかどうかを確認する時間を示している。プロダクトへの新しい変更を実装する際、スクラムチームが各ステージにどれだけの時間を費やすべきかについてのルールはない。あるステージに到達して、何かを見落とした前のステージに戻る必要があることに気づくかもしれない。

![Holistic Testing Model, copyright 2025, Janet Gregory and Lisa Crispin](/holistic-testing/2026.1/images/holistic-testing-model.jpg)

<!-- The next figure shows the same Holistic Testing Model with example testing activities. These are only examples, not necessarily best practices. Different Scrum Teams may do different activities, at different times, depending on their context. The key is to have effective conversations about testing and quality, with the whole team and Supporters, throughout the development cycle. Continuous improvement through small experiments and short feedback loops is the focus. Each Scrum Team needs to plan a testing strategy that includes all the necessary activities at the right time - throughout the development cycle. -->

次の図は、テスト活動の例を含む同じホリスティックテスティングモデルを示している。これらは例にすぎず、必ずしもベストプラクティスではない。異なるスクラムチームは、そのコンテキストに応じて、異なる時期に異なる活動を行うことがある。重要なのは、開発サイクル全体を通じて、チーム全体とサポーターとともに、テストと品質について効果的な会話を行うことである。小さな実験と短いフィードバックループによる継続的改善が焦点である。各スクラムチームは、開発サイクル全体を通じて、適切なタイミングで必要なすべての活動を含むテスト戦略を計画する必要がある。

<!-- Let's walk through the different stages of the model, which are basically the stages of the modern software development life cycle. Software development is an infinite loop, and new changes often begin with discovery, so we will start there. -->

モデルのさまざまなステージを見ていこう。これらは基本的に現代のソフトウェア開発ライフサイクルのステージである。ソフトウェア開発は無限ループであり、新しい変更は多くの場合、発見から始まるので、そこから始めよう。

![Holistic Testing Model with Example Testing Activities](/holistic-testing/2026.1/images/holistic-testing-model-example-testing-activities.jpg)

<!-- ## **Testing Early \- Discover and Plan** -->

## 早期のテスト - 発見と計画 {#testing-early-discover-and-plan}

<!-- Frequent delivery of small, sustainable changes is the key for software teams to continually deliver new value to customers. As Google's DORA research has shown over several years: -->

小さく持続可能な変更を頻繁にデリバリーすることが、ソフトウェアチームが継続的に顧客に新しい価値を提供するための鍵である。Googleの DORA リサーチが数年にわたって示してきたように：

<!-- _"Working in small batches" is a long-time DORA Capability, which refers to the degree to which teams break down their changes into manageable units that can be quickly tested and evaluated._ " [3] -->

_「小さなバッチで作業する」は長年の DORA ケイパビリティであり、チームが変更を素早くテストおよび評価できる管理可能な単位に分解する程度を指す。_ [3]

<!-- Teams need those quick feedback loops to build quality in. That means preventing bugs by brainstorming about the value to customers and risks as soon as we start working on a new change. -->

チームは品質を作り込むためにその迅速なフィードバックループを必要としている。つまり、新しい変更に取り組み始めるとすぐに、顧客への価値とリスクについてブレインストーミングすることでバグを予防することを意味する。

<!-- Teams do lots of testing in these stages – testing ideas, understanding user needs, looking for risks, and thinking about how to mitigate them. Together with Supporters, Stakeholders, and customers, they discuss the user needs. They ask questions like "What problem is this solving for the customer? What is the main value this capability should provide?" -->

チームはこれらのステージで多くのテストを行う - アイデアのテスト、ユーザーニーズの理解、リスクの探索、それらを軽減する方法の検討。サポーター、ステークホルダー、顧客とともに、ユーザーニーズについて議論する。「これは顧客のどのような問題を解決するのか？この機能が提供すべき主な価値は何か？」といった質問をする。

<!-- [Google's 2024 DORA research report](https://dora.dev/research/2024/dora-report/) [4] found that "alignment between what Product Developers build and what users need allows employees and organizations to thrive." [3]. Their research showed that prioritizing the end user helps development teams and their organizations perform better. Investing time in structured conversations to plan new features pays off by making sure the right capabilities are delivered on the first try. -->

[Googleの2024年DORAリサーチレポート](https://dora.dev/research/2024/dora-report/) [4] は、「プロダクト開発者が構築するものとユーザーが必要とするものの整合性が、従業員と組織の繁栄を可能にする」ことを発見した [3]。彼らの研究は、エンドユーザーを優先することが開発チームとその組織のパフォーマンス向上に役立つことを示した。新機能を計画するための構造化された会話に時間を投資することで、最初の試みで適切な機能を提供できるようになり、その投資は報われる。

<!-- They use visual frameworks such as risk storming [5] to identify potential risks and brainstorm ways to mitigate them. They might choose to mitigate them through automated tests or by monitoring and [observability](https://charity.wtf/2020/03/03/observability-is-a-many-splendored-thing/) [6]. For example, teams use [Open Telemetry](https://opentelemetry.io/) [7] to ensure they capture all data and events needed to understand any unexpected problems [8]. -->

彼らはリスクストーミング [5] などの視覚的フレームワークを使用して潜在的なリスクを特定し、それらを軽減する方法をブレインストーミングする。自動テストや、モニタリングと[オブザーバビリティ](https://charity.wtf/2020/03/03/observability-is-a-many-splendored-thing/) [6] によってリスクを軽減することを選択するかもしれない。例えば、チームは [Open Telemetry](https://opentelemetry.io/) [7] を使用して、予期しない問題を理解するために必要なすべてのデータとイベントを確実に取得する [8]。

<!-- Prioritizing the top risks and quality attributes helps the Scrum Team plan how to mitigate them. They can make sure they build in the appropriate levels of attributes, such as performance, availability, and security, that the business and customers require. This enables the creation of appropriate acceptance and outcome criteria for each new feature. -->

上位のリスクと品質特性を優先順位付けすることで、スクラムチームはそれらを軽減する方法を計画できる。ビジネスと顧客が要求するパフォーマンス、可用性、セキュリティなどの適切なレベルの特性を確実に作り込むことができる。これにより、各新機能に対する適切な受け入れ基準とアウトカム基準の作成が可能になる。

<!-- Here's an example of a risk brainstorming exercise done by members of the delivery Scrum Team and Stakeholders whose company has a "horse and donkey motels" web-based application. They considered risks around a new product backlog item (in story format) to add the capability for customers to cancel their booking for their equine and people accommodation. -->

以下は、「馬とロバのモーテル」Webベースアプリケーションを持つ会社のデリバリースクラムチームメンバーとステークホルダーが行ったリスクブレインストーミング演習の例である。彼らは、顧客が馬と人の宿泊予約をキャンセルできる機能を追加するための新しいプロダクトバックログアイテム（ストーリー形式）に関するリスクを検討した。

!["Brisk de-risking" board example for an equine motel company application](/holistic-testing/2026.1/images/brisk-derisking-board-example.png)

<!-- These planning discussions often show that a proposed feature is too big and needs to be broken down into smaller components. The goal of this stage is to break each new feature into small, testable product backlog items. -->

これらの計画の議論では、提案された機能が大きすぎて、より小さなコンポーネントに分割する必要があることがよく示される。このステージの目標は、各新機能を小さくテスト可能なプロダクトバックログアイテムに分割することである。

<!-- ## **Seek to Understand** -->

## 理解を追求する {#seek-to-understand}

<!-- Once the Scrum Team, in collaboration with Stakeholders and Supporters, has created those small, testable product backlog itemsstories, it's time to dig into the details and get a shared understanding of each onestory. In Refinement and Sprint Planning, Product Developers and Stakeholders discuss the goal, the business rules, and the concrete example for each business rule. -->

スクラムチームがステークホルダーやサポーターと協力して、これらの小さくテスト可能なプロダクトバックログアイテム（ストーリー）を作成したら、詳細を掘り下げて各ストーリーの共有理解を得る時である。リファインメントとスプリントプランニングでは、プロダクト開発者とステークホルダーがゴール、ビジネスルール、各ビジネスルールの具体例について議論する。

<!-- To work as effectively as possible, they use visual frameworks like [example mapping](https://cucumber.io/blog/bdd/example-mapping-introduction/) [9]. These structured frameworks keep conversations on track and help everyone reframe the problem and see what emerges. The Scrum Team members also identify the data and events to capture through logging and instrumentation in the code, so they can monitor and understand what happens in production after deployment. -->

できるだけ効果的に作業するために、[エグザンプルマッピング](https://cucumber.io/blog/bdd/example-mapping-introduction/) [9] などの視覚的フレームワークを使用する。これらの構造化されたフレームワークは会話を軌道に乗せ、全員が問題を再構成し、何が創発するかを見るのに役立つ。スクラムチームメンバーはまた、コード内のログ記録と計装を通じて取得するデータとイベントを特定し、デプロイ後にプロダクションで何が起こるかを監視して理解できるようにする。

<!-- These structured conversations let the Scrum Team plan how to mitigate the top priority risks for each story. They can create acceptance and outcome criteria that ensure they deliver what customers and Stakeholders value most. -->

これらの構造化された会話により、スクラムチームは各ストーリーの最優先リスクを軽減する方法を計画できる。顧客とステークホルダーが最も価値を置くものを確実に提供する受け入れ基準とアウトカム基準を作成できる。

<!-- Here's a sample example map from a Scrum Team working on a web-based app that allows company employees to schedule Scrum Team meetings. This map was created during a short session before the official sprint planning meeting. These sessions are sometimes known as Power of Three or Three Amigos, where people with product, development, and quality domain skills collaborate [10]. In this case, the Product Owner, the quality engineer, and two programmers discuss each product backlog item that the Scrum Team would include in the subsequent Sprint Planning. -->

以下は、会社の従業員がスクラムチームミーティングをスケジュールできるWebベースアプリに取り組むスクラムチームからのエグザンプルマップのサンプルである。このマップは、正式なスプリントプランニングミーティングの前の短いセッション中に作成された。これらのセッションは、プロダクト、開発、品質の各ドメインスキルを持つ人々が協力する「パワー・オブ・スリー」または「スリーアミーゴス」として知られることがある [10]。この場合、プロダクトオーナー、品質エンジニア、2人のプログラマーが、スクラムチームがその後のスプリントプランニングに含めるであろう各プロダクトバックログアイテムについて議論する。

<!-- The yellow card is the product backlog item. Blue cards contain business rules, and green cards provide examples that illustrate the desired behavior for the business rules. The red cards have questions that need to be answered before the Sprint Planning. -->

黄色のカードはプロダクトバックログアイテムである。青いカードにはビジネスルールが含まれ、緑のカードはビジネスルールの望ましい振る舞いを示す例を提供する。赤いカードには、スプリントプランニングの前に回答する必要がある質問がある。

![Sample example map](/holistic-testing/2026.1/images/sample-map.png)

<!-- ## **Testing Activities While We Build** -->

## 構築中のテスト活動 {#testing-activities-while-we-build}

<!-- Once everyone is on the same page as to how the new change should behave, the Scrum Team starts building … coding, automating, testing – not necessarily in that order. Optimally, they use good practices like [test-driven development](https://martinfowler.com/bliki/TestDrivenDevelopment.html) (TDD) [13] to get well-designed, operable, testable code. -->

新しい変更がどのように振る舞うべきかについて全員が同じ認識を持ったら、スクラムチームは構築を開始する...コーディング、自動化、テスト - 必ずしもその順序ではない。最適には、[テスト駆動開発](https://martinfowler.com/bliki/TestDrivenDevelopment.html)（TDD）[13] などの良いプラクティスを使用して、適切に設計され、操作可能で、テスト可能なコードを得る。

<!-- Janet Gregory often says: -->

Janet Gregory はよくこう言う：

<!-- _Throw away the 'then' in 'code, then test'. Replace it with 'and'. And maybe, also reverse the order to say, 'test AND code'. Put the test first. [11]_ -->

_「コードしてからテスト」の「から」を捨てなさい。それを「と」に置き換えなさい。そしてたぶん、順序を逆にして「テストとコード」と言いなさい。テストを先に置きなさい。[11]_

<!-- In the build stage, team members guide development with business-facing examples, using techniques like [behavior-driven development](https://www.manning.com/books/effective-behavior-driven-development) [12]. These examples are turned into tests, which focus on quality and value from a business perspective. The whole Scrum Team can participate in these activities, making sure they build the right thing, in the right way. -->

構築ステージでは、チームメンバーは[ビヘイビア駆動開発](https://www.manning.com/books/effective-behavior-driven-development) [12] などの技法を使用して、ビジネス向けの例で開発をガイドする。これらの例はテストに変換され、ビジネスの観点から品質と価値に焦点を当てる。スクラムチーム全体がこれらの活動に参加でき、正しいものを正しい方法で構築していることを確認する。

<!-- The Scrum Team automates tests as appropriate, at the appropriate levels – unit, API, workflow. The whole Scrum Team and possibly the Stakeholders are involved. As with earlier stages, they collaborate to prevent customer pain and to embed telemetry into the product to capture the data that will let us learn from production. -->

スクラムチームは適切なレベル - ユニット、API、ワークフロー - で適切にテストを自動化する。スクラムチーム全体と、場合によってはステークホルダーも関与する。前のステージと同様に、彼らは顧客の苦痛を予防し、プロダクションから学ぶことができるデータを取得するためにプロダクトにテレメトリを組み込むために協力する。

<!-- ## **Deploying and releasing** -->

## デプロイとリリース {#deploying-and-releasing}

<!-- When new changes are deployed to production-like test environments, Scrum Team members can do more feature-level testing. The continuous integration pipelines run automated regression tests. It's a key time to test for the high-priority quality attributes, also known as non-functional requirements, such as security, accessibility, and performance. -->

新しい変更がプロダクションに似たテスト環境にデプロイされると、スクラムチームメンバーはより多くの機能レベルのテストを行うことができる。継続的インテグレーションパイプラインは自動リグレッションテストを実行する。セキュリティ、アクセシビリティ、パフォーマンスなど、非機能要件としても知られる優先度の高い品質特性をテストする重要な時期である。

<!-- It's also an opportunity to check that new instrumentation is capturing the right data, and new or updated dashboards and alerts are accurate. This will help measure whether the Scrum Team achieves elements of its Definition of Outcome Done. They also ensure they are ready to support the new changes in production, so we can test logging and dashboards. -->

これはまた、新しい計装が適切なデータを取得しているか、新しいまたは更新されたダッシュボードとアラートが正確であるかを確認する機会でもある。これは、スクラムチームがアウトカム完成の定義の要素を達成しているかどうかを測定するのに役立つ。また、プロダクションで新しい変更をサポートする準備ができていることを確認するため、ログ記録とダッシュボードをテストできる。

<!-- A fast and reliable deployment pipeline is a necessity. It provides fast feedback, especially for Scrum Teams working towards continuous delivery. Once a feature becomes usable, Scrum Teams can conduct human-centric activities such as exploratory and accessibility testing. -->

高速で信頼性の高いデプロイパイプラインは必須である。特に継続的デリバリーに向けて取り組むスクラムチームにとって、迅速なフィードバックを提供する。機能が使用可能になると、スクラムチームは探索的テストやアクセシビリティテストなどの人間中心の活動を行うことができる。

<!-- Modern Scrum Teams use release strategies to enable deploying changes to production without releasing them to users. Examples of popular release strategies include: -->

現代のスクラムチームは、変更をユーザーにリリースせずにプロダクションにデプロイすることを可能にするリリース戦略を使用する。一般的なリリース戦略の例には以下が含まれる：

<!-- - [Release feature toggles / flags](https://martinfowler.com/articles/feature-toggles.html) [14]: adding booleans to the code so the Scrum Team can opt to show the new change to some or all external customers, or keep it hidden. Similar toggles, called "experiment toggles", are often used for A/B testing. -->

- [リリースフィーチャートグル / フラグ](https://martinfowler.com/articles/feature-toggles.html) [14]: スクラムチームが新しい変更を一部またはすべての外部顧客に表示するか、非表示のままにするかを選択できるように、コードにブール値を追加する。「実験トグル」と呼ばれる同様のトグルは、A/Bテストによく使用される。

<!-- - [Blue-Green deployment](https://octopus.com/devops/software-deployments/blue-green-deployment/) [15]: Two identical production environments, one live and accessible to customers, one idle and only accessible internally, referred to as "blue" and "green". The team can deploy to the idle environment, run additional tests, and switch customer traffic to the one with the new deployment. -->

- [ブルーグリーンデプロイメント](https://octopus.com/devops/software-deployments/blue-green-deployment/) [15]: 2つの同一のプロダクション環境で、1つは稼働中で顧客がアクセス可能、もう1つはアイドル状態で内部からのみアクセス可能であり、「ブルー」と「グリーン」と呼ばれる。チームはアイドル環境にデプロイし、追加のテストを実行し、顧客トラフィックを新しいデプロイメントのある環境に切り替えることができる。

<!-- - [Rolling deployment](https://octopus.com/devops/software-deployments/rolling-deployment/) [16]: Deployment of a new release candidate is staggered to a subset of servers, one or a few at a time. If any problems are detected, the deployment can be halted and rolled back. -->

- [ローリングデプロイメント](https://octopus.com/devops/software-deployments/rolling-deployment/) [16]: 新しいリリース候補のデプロイメントは、サーバーのサブセットに1台または数台ずつ段階的に行われる。問題が検出された場合、デプロイメントを停止してロールバックできる。

<!-- The Scrum Team, sometimes including programmers, testers/quality engineers, operations specialists, and others, discusses which release strategies would work best in their context. They can experiment with different approaches, define a hypothesis, and decide how they will measure success. -->

スクラムチームは、プログラマー、テスター/品質エンジニア、運用スペシャリストなどを含むこともあり、どのリリース戦略が彼らのコンテキストで最も効果的かを議論する。さまざまなアプローチで実験し、仮説を定義し、成功をどのように測定するかを決定できる。

<!-- Depending on their context, the Scrum Team can safely do testing in production that couldn't be done effectively in test environments. We can gradually roll out changes to more customers while closely monitoring for any issues. -->

コンテキストに応じて、スクラムチームはテスト環境では効果的に行えないテストをプロダクションで安全に行うことができる。問題を注意深く監視しながら、より多くの顧客に変更を段階的にロールアウトできる。

<!-- ## **Observing and learning** -->

## 観察と学習 {#observing-and-learning}

<!-- Once features are in production, Scrum Teams can observe customer actions and reactions. The telemetry, based on instrumentation planned in the early stages, is used here. What the team learns from observability and analytics helps the organization prioritize the next changes. Often, they will observe something completely unexpected, like customers using a new feature in an unintended way. That's an opportunity to try some new experiments in subsequent development cycles. -->

機能がプロダクションに入ると、スクラムチームは顧客の行動と反応を観察できる。初期段階で計画された計装に基づくテレメトリがここで使用される。チームがオブザーバビリティと分析から学んだことは、組織が次の変更を優先順位付けするのに役立つ。多くの場合、顧客が新機能を意図しない方法で使用するなど、まったく予期しないことを観察する。それは、その後の開発サイクルで新しい実験を試す機会である。

<!-- Together with the Guiding Coalition, we can design experiments to improve our process and product. We move on to the next iteration through the cycle, starting over with the next discovery stage. -->

指導連合とともに、プロセスとプロダクトを改善するための実験を設計できる。次の発見ステージから再開して、サイクルを通じて次のイテレーションに進む。

<!-- ## **Summing up** -->

## まとめ {#summing-up}

<!-- Testing activities on the left side of the Holistic Testing loop aim to prevent defects in the code that could cost the business and its customers time and money. This is the quickest feedback, and it happens when team members with diverse skills and experience work together with the Supporters. -->

ホリスティックテスティングループの左側のテスト活動は、ビジネスとその顧客に時間とお金のコストをかける可能性のあるコードの欠陥を予防することを目的としている。これは最も迅速なフィードバックであり、多様なスキルと経験を持つチームメンバーがサポーターと一緒に作業するときに発生する。

<!-- This collaboration continues on the right side of the loop, finding defects, missed capabilities, and deficiencies in quality attributes as quickly as possible. Learning how customers use the new changes is slower feedback; it's more expensive. If the team has built in the right telemetry and infrastructure, they can respond quickly to problems. Everyone on a Scrum Team can contribute to every stage of the Holistic Testing cycle. -->

このコラボレーションはループの右側でも続き、欠陥、見落とされた機能、品質特性の不足をできるだけ迅速に発見する。顧客が新しい変更をどのように使用するかを学ぶことは、より遅いフィードバックであり、より高価である。チームが適切なテレメトリとインフラストラクチャを作り込んでいれば、問題に迅速に対応できる。スクラムチームの全員が、ホリスティックテスティングサイクルのすべてのステージに貢献できる。

<!-- ## **The Quality Engineer Competency** -->

## 品質エンジニアのコンピテンシー {#the-quality-engineer-competency}

<!-- Everyone on a Scrum Team should have a testing mindset and engage in testing activities. They build quality in. Each Scrum Team member has their own deep skills - not everyone starts out with a testing mindset and testing skills. This diversity of skill sets, experience, and background helps the Scrum Team perform better. -->

スクラムチームの全員がテストマインドセットを持ち、テスト活動に従事すべきである。彼らは品質を作り込む。各スクラムチームメンバーには独自の深いスキルがある - 全員がテストマインドセットとテストスキルを持って始めるわけではない。このスキルセット、経験、バックグラウンドの多様性が、スクラムチームのパフォーマンス向上に役立つ。

<!-- A software quality engineer (QE) partners with product, development, and operations specialists to embed quality throughout the entire life cycle. Ideally, each Scrum Team has QE skills. In many organizations, a senior QE may support multiple Scrum Teams in a consulting role to build up QE skills. The QE helps all Scrum Team members learn skills to improve quality throughout the development cycle. -->

ソフトウェア品質エンジニア（QE）は、プロダクト、開発、運用のスペシャリストと連携して、ライフサイクル全体を通じて品質を組み込む。理想的には、各スクラムチームがQEスキルを持っている。多くの組織では、シニアQEがコンサルティングの役割で複数のスクラムチームをサポートし、QEスキルを構築することがある。QEは、すべてのスクラムチームメンバーが開発サイクル全体を通じて品質を向上させるスキルを学ぶのを助ける。

<!-- Quality engineers, who may also be called quality advocates, testers, or other labels, collaborate across disciplines to help manage risk, facilitate discussion, and align on quality goals. They are strategic contributors who improve processes and help the Scrum Team build process and product quality. -->

品質エンジニアは、品質アドボケイト、テスター、またはその他の呼称で呼ばれることもあり、リスク管理、議論の促進、品質目標の整合を支援するために分野を超えて協力する。彼らはプロセスを改善し、スクラムチームがプロセスとプロダクトの品質を構築するのを助ける戦略的な貢献者である。

<!-- Key activities of a quality engineer in a Scrum Team could include: -->

スクラムチームにおける品質エンジニアの主要な活動には以下が含まれる：

<!-- - Design test frameworks and tools -->
<!-- - Track metrics and drive continuous improvement -->
<!-- - Participate in and even facilitate retrospectives to find ways to prevent problems from recurring -->
<!-- - Experiment with new practices -->
<!-- - Coach Scrum Teams as they look for ways to improve product and process quality -->
<!-- - Integrate feedback from customers -->

- テストフレームワークとツールの設計
- メトリクスの追跡と継続的改善の推進
- 問題の再発を防ぐ方法を見つけるためのレトロスペクティブへの参加、さらにはファシリテーション
- 新しいプラクティスの実験
- プロダクトとプロセスの品質を向上させる方法を探すスクラムチームのコーチング
- 顧客からのフィードバックの統合

<!-- Quality is the responsibility of everyone on the Scrum Team, as well as the Stakeholders and Supporters. The Quality Engineer enables the Scrum Team to deliver reliable, valuable software. And, every Scrum Team member actively engages in testing activities that help build quality in. -->

品質は、ステークホルダーやサポーターだけでなく、スクラムチームの全員の責任である。品質エンジニアは、スクラムチームが信頼性の高い価値あるソフトウェアを提供できるようにする。そして、すべてのスクラムチームメンバーが、品質を作り込むのに役立つテスト活動に積極的に従事する。

<!-- ## References -->

## 参考文献 {#references}

[1] Gregory, J. and Crisipin L. (2010) _ATDD vs. BDD vs. Specification by Example vs …_ 31 August. Available at: <https://janetgregory.ca/atdd-vs-bdd-vs-specification-by-example-vs/> (Accessed: 19 December 2025)

[2] Gregory, J. & Crispin, L., 2025. Quality Attributes – those pesky "non-functional" requirements. Agile Testing Fellowship, 17 March. Available at: <https://agiletestingfellow.com/blog/post/quality-attributes-those-pesky-non-functional-requirements> (Accessed 29 December 2025)

[3] Forsgren, N., Humble, J., Kim, G. & the DORA Team, 2025. DORA 2025 State of AI-Assisted Software Development Report. Google Cloud. Available at: <https://cloud.google.com/devops/state-of-devops> (Accessed 29 December 2025)

[4] DORA, 2024. DORA Report 2024. Google Cloud. Available at: <https://dora.dev/research/2024/dora-report/> (Accessed 29 December 2025)

[5] RiskStorming, n.d. RiskStorming. Available at: <https://riskstormingonline.com/> (Accessed 29 December 2025)

[6] Majors, C., 2020. Observability is a many-splendored thing. Charity.wtf, 3 March. Available at: <https://charity.wtf/2020/03/03/observability-is-a-many-splendored-thing/> (Accessed 29 December 2025)

[7] OpenTelemetry, n.d. OpenTelemetry. Cloud Native Computing Foundation. Available at: <https://opentelemetry.io/> (Accessed 29 December 2025)

[8] Sridharan, C., 2017. Monitoring and observability. Medium, 5 September. Available at: [https://copyconstruct.medium.com/monitoring-and-observability-8417d1952e1c](https://copyconstruct.medium.com/monitoring-and-observability-8417d1952e1c) (Accessed 29 December 2025)

[9] Cucumber Ltd., n.d. Example Mapping: an introduction. Cucumber Blog. Available at: <https://cucumber.io/blog/bdd/example-mapping-introduction/> (Accessed 29 December 2025)

[10] Wynne, M. & Hellesøy, A., 2012. The Cucumber Book: Behaviour-Driven Development for Testers and Developers. Dallas, TX: Pragmatic Bookshelf.

[11] Gregory, J. & Crispin, L., 2015. Holistic Testing: Weave Quality Into Your Product. Upper Saddle River, NJ: Addison-Wesley Professional.

[12] Smart, J.F., Molina, J. & Farcic, A., 2014. Effective Behavior-Driven Development. Shelter Island, NY: Manning Publications. Available at: <https://www.manning.com/books/effective-behavior-driven-development> (Accessed 29 December 2025)

[13] Fowler, M., 2014. Test-Driven Development. MartinFowler.com. Available at: <https://martinfowler.com/bliki/TestDrivenDevelopment.html> (Accessed 29 December 2025)

[14] Fowler, M., 2017. Feature Toggles (aka Feature Flags). MartinFowler.com. Available at: <https://martinfowler.com/articles/feature-toggles.html> (Accessed 29 December 2025)

[15] Octopus Deploy, n.d. Blue-green deployment. Available at: <https://octopus.com/devops/software-deployments/blue-green-deployment/> (Accessed 29 December 2025)

[16] Octopus Deploy, n.d. Rolling deployment. Available at: <https://octopus.com/devops/software-deployments/rolling-deployment/> (Accessed 29 December 2025)
