---
title: プロダクト思考（SGEPの拡張）
subtitle: アウトプットからアウトカムへ – 真のインパクトを生むプロダクトマネジメント
description: 現代のスクラムはプロダクト思考を要求し、チームがアウトプットの納品からアウトカムと長期的インパクトのオーナーシップへと移行することを促します。これはエビデンス、フィードバックループ、継続的学習によって支えられ、SGEPのアウトプット完成の定義とアウトカム完成の定義、およびエビデンスベースドマネジメントによってサポートされます。
keywords:
  - アウトカムオーナーシップ
  - インパクト測定
  - エビデンスベースドマネジメント
  - プロダクト運用モデル
author:
  - Ralph Jocham
  - Magdalena Firlit
translators:
  - Claude AI
  - Takeshi Kawaguti
date: 2026-01-18T09:00:00Z
type: guide
lang: ja
mainfont: "Times New Roman"
sansfont: "Arial"
monofont: "Courier New"
forked_from: scrum-guide-expansion-pack/2025.6
aliases:
  - /ja/product-thinking/2026.1/
sitemap:
  priority: 0.7
---

<!-- License/Copyright: [CC BY-NC-ND 4.0](https://creativecommons.org/licenses/by-nc-nd/4.0/)
Note: This section is included in its original, unaltered form with permission under the terms of the [CC BY-NC-ND 4.0](https://creativecommons.org/licenses/by-nc-nd/4.0/) license. No changes have been made. -->

ライセンス/著作権: [CC BY-NC-ND 4.0](https://creativecommons.org/licenses/by-nc-nd/4.0/)
注記: このセクションは [CC BY-NC-ND 4.0](https://creativecommons.org/licenses/by-nc-nd/4.0/) ライセンスの条件に基づき、許可を得て原文のまま収録されています。変更は加えられていません。

---

<!-- ## Introduction -->

## はじめに {#introduction}

<!-- In 2001, seventeen software practitioners gathered in Snowbird, Utah, and wrote what became known as the Agile Manifesto. It was a short declaration of values and principles that guided a generation of software teams [^1]. Almost a decade later, in 2010, Kent Beck — one of the original signatories — spoke at the Startup Lessons Learned Conference and reflected on how he might have written the Manifesto differently or how it should have been then [^2]. His version placed new emphasis on team vision, validated learning, customer discovery, and initiating change. -->

2001年、17人のソフトウェア実践者がユタ州スノーバードに集まり、後にアジャイルマニフェストとして知られるものを書きました。それは一世代のソフトウェアチームを導いた価値と原則の短い宣言でした[^1]。約10年後の2010年、署名者の一人であるKent Beckは Startup Lessons Learned Conferenceで講演し、マニフェストをどのように異なる形で書いたか、あるいは当時どうあるべきだったかについて振り返りました[^2]。彼のバージョンは、チームビジョン、検証された学習、顧客発見、変化の主導に新たな重点を置いていました。

<!-- He expressed this shift in values as follows: -->

彼はこの価値観の変化を次のように表現しました:

<!-- **Team Vision and Discipline** over **Individuals and Interactions** over **Processes and Tools**
**Validated Learning** over **Working Software** over **Comprehensive Documentation**
**Customer Discovery** over **Customer Collaboration** over **Contract Negotiation**
**Initiating Change** over **Responding to Change** over **Following a Plan** -->

**チームビジョンと規律** よりも **個人と対話** よりも **プロセスとツール**
**検証された学習** よりも **動くソフトウェア** よりも **包括的なドキュメント**
**顧客発見** よりも **顧客との協調** よりも **契約交渉**
**変化の主導** よりも **変化への対応** よりも **計画に従うこと**

<!-- Why this change of mind? The world of 2001 was very different from the world of 2010, and even more so from today. In 2001, software was often delivered by consulting companies, called vendors. A business would hire these vendors because it lacked either the capacity or the expertise to build software in-house. The vendor's job was simple: build what the client asked for, deliver it on time, and maintain quality. In that context, success meant output delivered according to specification. -->

なぜこのような考えの変化があったのでしょうか？2001年の世界は2010年の世界とは大きく異なり、今日とはさらに異なっています。2001年には、ソフトウェアはベンダーと呼ばれるコンサルティング会社によって納品されることが多くありました。企業は社内でソフトウェアを構築する能力や専門知識がなかったため、これらのベンダーを雇いました。ベンダーの仕事はシンプルでした：クライアントが求めるものを構築し、期限通りに納品し、品質を維持すること。その文脈では、成功とは仕様通りに納品されたアウトプットを意味しました。

<!-- That was in 2010. For reflection purposes only, one might wonder what a comparable emphasis could look like in 2026 [^22]. -->

それは2010年のことでした。振り返りの目的のみで、2026年における同様の強調がどのようなものになりうるか考えてみましょう[^22]。

<!-- **People Empowerment Improvement** over **Individuals and Interactions** over **Processes and Tools**
**Value Improvement** over **Working Product** over **Comprehensive Documentation**
**Insight Improvement** over **Customer Collaboration** over **Contract Negotiation**
**Capability Improvement** over **Responding to Change** over **Following a Plan** -->

**人々のエンパワーメント向上** よりも **個人と対話** よりも **プロセスとツール**
**価値の向上** よりも **動くプロダクト** よりも **包括的なドキュメント**
**洞察の向上** よりも **顧客との協調** よりも **契約交渉**
**能力の向上** よりも **変化への対応** よりも **計画に従うこと**

<!-- _In a nutshell:_
_**Short- to long-term Work Climate, Learning, Outcomes,** **and Impact** over **Outputs**_
_over **Activities and 'Resources'**_ -->

_一言で言えば:_
_**短期から長期の職場環境、学習、アウトカム、そしてインパクト** よりも **アウトプット**_
_よりも **活動と「リソース」**_

<!-- This reflection revealed a deeper truth: **output is not the same as outcome** [^17]. Delivering features is not the same as creating value. And in today's continuous innovation economy, where companies live or die based on customer engagement, product adoption, and financial sustainability, it is no longer enough to just deliver a product. Effective product work requires connecting inputs to activities, activities to outputs, outputs to outcomes, and outcomes to impact [^3]. -->

この振り返りは、より深い真実を明らかにしました：**アウトプットはアウトカムと同じではない**[^17]。機能を納品することは価値を創造することと同じではありません。そして、顧客エンゲージメント、プロダクトの採用、財務的な持続可能性に基づいて企業が存亡を分ける今日の継続的イノベーション経済において、単にプロダクトを納品するだけでは十分ではありません。効果的なプロダクト作業には、インプットを活動に、活動をアウトプットに、アウトプットをアウトカムに、そしてアウトカムをインパクトに結びつけることが必要です[^3]。

<!-- This shift is not just about **what** is done, but about **why** and **for whom** it is done [^4]. Too often, teams obsess over delivery speed or process optimization while losing sight of the purpose behind their work. The original intent of Agile, when applied with the **why** and **who** in mind, forces us to ask: _How does this activity or output help customers and strengthen the company's future?_ That question grounds day-to-day work in long-term impact. -->

この転換は単に**何を**行うかについてではなく、**なぜ**、**誰のために**行うかについてです[^4]。あまりにも頻繁に、チームは納品スピードやプロセスの最適化に執着しながら、作業の背後にある目的を見失っています。アジャイルの本来の意図は、**なぜ**と**誰のために**を念頭に置いて適用されたとき、私たちに問いかけることを強制します：_この活動やアウトプットは顧客をどのように助け、会社の将来をどのように強化するのか？_ この問いは日々の作業を長期的なインパクトに根付かせます。

![ロジックモデル - 拡張バリューチェーン](/product-thinking/images/value-chain-feedback-loop.png)

<!-- This document explores that shift. Using the lens of the Scrum Guide Expansion Pack (SGEP) [^14] and frameworks such as Evidence-Based Management (EBM), this analysis explains why product teams should shift from focusing on activities and outputs to intentionally owning outcomes and impacts [^5] -->

この文書はその転換を探求します。Scrum Guide Expansion Pack（SGEP）[^14]とEvidence-Based Management（EBM）などのフレームワークのレンズを使用して、この分析はプロダクトチームが活動とアウトプットへの注力から、意図的にアウトカムとインパクトを所有することへ転換すべき理由を説明します[^5]

<!-- ## Why the Agile Manifesto Looked Like It Did -->

## アジャイルマニフェストがああいう形になった理由 {#why-the-agile-manifesto-looked-like-it-did}

<!-- To understand why Kent Beck's 2010 version looked so different, the context of 2001 must be revisited. The authors of the Agile Manifesto were a potpourri of mostly consultants, software creators, experts, and thought leaders behind various upcoming practices. They were deeply involved in improving software development processes. Their business model was built on delivering software projects for paying clients. They were all proponents of making the software development process less formal or more lightweight and had been successful with it. They were trying to understand the common values and principles they all shared. And, since they didn't want to be known as "the lightweights", they chose the term "Agile" to best describe their shared mindset. -->

Kent Beckの2010年バージョンがなぜそれほど異なって見えたかを理解するためには、2001年の文脈を再訪する必要があります。アジャイルマニフェストの著者たちは、主にコンサルタント、ソフトウェア作成者、専門家、そして様々な新興プラクティスの背後にいるソートリーダーの寄せ集めでした。彼らはソフトウェア開発プロセスの改善に深く関わっていました。彼らのビジネスモデルは、支払いをするクライアントのためにソフトウェアプロジェクトを納品することに基づいていました。彼らは全員、ソフトウェア開発プロセスをより形式的でなく、あるいはより軽量にすることの支持者であり、それで成功を収めていました。彼らは全員が共有する共通の価値と原則を理解しようとしていました。そして、「軽量派」として知られたくなかったため、共有するマインドセットを最もよく表す言葉として「アジャイル」を選びました。

<!-- Think of a bank in 2000. The bank might need an online portal, but it didn't have a large development team. Instead, it hired a consultancy. The consultancy's product was not the software itself - it was the **service** of building software to order. Their success metric was: _did we deliver what the client asked for?_ -->

2000年の銀行を考えてみてください。銀行はオンラインポータルが必要かもしれませんが、大規模な開発チームを持っていませんでした。代わりに、コンサルタント会社を雇いました。コンサルタント会社のプロダクトはソフトウェアそのものではなく、注文に応じてソフトウェアを構築する**サービス**でした。彼らの成功指標は：_クライアントが求めたものを納品したか？_

<!-- From this perspective, the values of the Agile Manifesto made sense. For example: -->

この観点から、アジャイルマニフェストの価値は理にかなっていました。例えば：

<!-- - **Individuals and interactions over processes and tools** fit a consulting context, where client happiness was tied to good communication and a good vendor-client relationship.
- **Working software over comprehensive documentation** reassured clients that they would actually get usable code, the output.
- **Customer collaboration over contract negotiation** encouraged a flexible procurement with paying clients.
- **Responding to change over following a plan** allowed engagements to be grounded in Transparency, Inspection, and Adaptation. Put more simply, it requires staying aware of emerging changes and adjusting what is intended to be built based on what has been learned. -->

- **プロセスやツールよりも個人と対話を**は、クライアントの満足が良好なコミュニケーションと良好なベンダー・クライアント関係に結びついていたコンサルティングの文脈に適合しました。
- **包括的なドキュメントよりも動くソフトウェアを**は、クライアントに実際に使用可能なコード、つまりアウトプットを得られることを保証しました。
- **契約交渉よりも顧客との協調を**は、支払いをするクライアントとの柔軟な調達を奨励しました。
- **計画に従うことよりも変化への対応を**は、透明性、検査、適応に基づいた契約を可能にしました。より簡単に言えば、新たな変化を認識し、学んだことに基づいて構築しようとしているものを調整することが求められます。

<!-- Notice the orientation: everything is about delivering what the client wanted. In other words, the approach was **output‑focused**. The consultancy's job ended with delivering the requested output; whether that output actually improved the bank's business outcomes was left entirely to the bank. -->

方向性に注目してください：すべてはクライアントが望んだものを納品することについてです。言い換えれば、そのアプローチは**アウトプット中心**でした。コンサルタント会社の仕事は要求されたアウトプットを納品することで終わり、そのアウトプットが実際に銀行のビジネスアウトカムを改善したかどうかは、完全に銀行に委ねられていました。

<!-- Today, sadly, many companies outsource even more parts of their digital product development; essentially entrusting their corporate brains and backbone to someone else. For some, this could work, even in a long-term vendor relationship. However, for many successful companies, the way of thinking has changed. Critical products are no longer seen as projects to be delivered and then **kept alive or, worse, forgotten**. Instead, organizations expect continuous evolution, learning, and adaptation of their products, often referred to as a **product‑operating‑model** [^16]. Whether built in-house or with external partners, teams are now expected to go beyond output and take responsibility for **outcomes** and, ultimately, **business impact**. -->

今日、残念なことに、多くの企業はデジタルプロダクト開発のさらに多くの部分を外部委託しています。本質的に、企業の頭脳とバックボーンを他者に委ねています。一部の企業にとっては、長期的なベンダー関係であっても、これはうまくいく可能性があります。しかし、多くの成功した企業にとって、考え方は変わりました。重要なプロダクトは、納品されてから**維持されるか、さらに悪いことに忘れられる**プロジェクトとしてはもはや見られていません。代わりに、組織はプロダクトの継続的な進化、学習、適応を期待しており、これはしばしば**プロダクト運用モデル**と呼ばれます[^16]。社内で構築されるか外部パートナーと構築されるかにかかわらず、チームは今やアウトプットを超えて、**アウトカム**、そして最終的には**ビジネスインパクト**に責任を持つことが期待されています。

<!-- This shift also requires explicit Product Strategy: a clear direction of travel that explains who the product is for, what problem it solves, and how it creates advantage. Product Strategy is essential, but it will be covered in a separate SGEP document because it deserves its own depth. -->

この転換にはまた、明示的なプロダクト戦略も必要です：プロダクトが誰のためのものか、どのような問題を解決するか、どのように優位性を生み出すかを説明する明確な方向性です。プロダクト戦略は不可欠ですが、独自の深さに値するため、別のSGEP文書でカバーされます。

<!-- ## The Shift From Output to Outcome -->

## アウトプットからアウトカムへの転換 {#the-shift-from-output-to-outcome}

<!-- Shifting from an output-focused project delivery model—where success is measured by on-time, on-scope, on-budget delivery—to an outcome-oriented product operating model enables organizations to focus less on completed activities and more on the changes in behavior or conditions that indicate meaningful value realization and learning. -->

アウトプット中心のプロジェクト納品モデル（成功が期限通り、スコープ通り、予算通りの納品で測定される）から、アウトカム志向のプロダクト運用モデルへの転換により、組織は完了した活動への注力を減らし、意味のある価値実現と学習を示す行動や状況の変化により注力できるようになります。

<!-- _Leading indicators_ measure actions or conditions used in contexts, with the belief that they offer guidance on the direction of travel. Leading indicators do not predict outcomes.
_Lagging indicators_ measure results that have already happened — they show the actual impact of past actions [^34]. -->

_先行指標_は、進む方向についてのガイダンスを提供するという信念のもと、文脈で使用される行動や状況を測定します。先行指標はアウトカムを予測しません。
_遅行指標_は既に起こった結果を測定します—過去の行動の実際のインパクトを示します[^34]。

<!-- In complex domains, however, both leading and lagging indicators are shaped by interacting factors, so they should be treated as signals to learn or noise, not as definitive evidence of cause and effect. -->

しかし、複雑なドメインでは、先行指標と遅行指標の両方が相互作用する要因によって形作られるため、原因と結果の決定的なエビデンスとしてではなく、学習のためのシグナルまたはノイズとして扱うべきです。

<!-- Inputs are often shown as the first step. However, something happens before that first step is taken, the motivation to go through the effort. There could be a theory or a result to achieve [^31]. Essentially, there are general assumptions about a better future. -->

インプットはしばしば最初のステップとして示されます。しかし、その最初のステップが踏み出される前に何かが起こります。努力を経る動機です。達成すべき理論や結果があるかもしれません[^31]。本質的に、より良い未来についての一般的な仮定があります。

<!-- - **Assumption** — In the product world, it is about the challenges people have, whether they complain about them or not. The things that people love and desire. These 'needs', combined with an understanding of the technologies used to build products and deliver services, form the seeds of innovation. Solving a problem that people already recognize - using a solution they can readily imagine - is one thing. True innovation is meeting a need people did not realize they had, with a solution they could not have anticipated. This is often described as a core driver of personal and business success. -->

- **仮定** — プロダクトの世界では、人々が抱える課題についてです。彼らがそれについて不満を言うかどうかにかかわらず。人々が愛し、望むもの。これらの「ニーズ」は、プロダクトを構築しサービスを提供するために使用される技術の理解と組み合わさって、イノベーションの種を形成します。人々がすでに認識している問題を、彼らが容易に想像できる解決策で解決することは一つのことです。真のイノベーションとは、人々が気づいていなかったニーズを、彼らが予期できなかった解決策で満たすことです。これはしばしば個人とビジネスの成功の核心的な推進力として説明されます。

<!-- Following through, let's take a closer look at the value chain, which can be seen as a feedback loop with various learning exit points and starting points, not necessarily linear. -->

引き続き、バリューチェーンをより詳しく見てみましょう。これは様々な学習の出口と開始点を持つフィードバックループとして見ることができ、必ずしも線形ではありません。

<!-- - **Inputs** — Skills, knowledge (including learning from past decisions like outcome, impact, and experiment results), budget, working hours, and tools such as laptops, AI, software, and systems that enable the work. Also, feature requests, to-do lists, action plans, Increments, standards, and sometimes even bug reports can be considered as Inputs. Context matters. Inputs are easy to control. -->

- **インプット** — スキル、知識（アウトカム、インパクト、実験結果など過去の意思決定からの学習を含む）、予算、労働時間、そしてラップトップ、AI、ソフトウェア、作業を可能にするシステムなどのツール。また、機能リクエスト、ToDoリスト、アクションプラン、インクリメント、標準、時にはバグレポートもインプットと見なすことができます。文脈が重要です。インプットは制御しやすいものです。

<!-- Inputs, activities, outputs, outcomes, and impact often take into account some assumptions, such as what we observe in the world. The challenges people have, whether they complain about them or not. The things that people love and desire. These needs, combined with what we understand about the technology we use to build things and create services, are the seeds of innovation. It's one thing to solve a problem people know they have with what they imagine as a solution. It's true innovation: fulfilling a need they didn't know they had with a solution they could never have imagined. This is the real secret to personal and business success. -->

インプット、活動、アウトプット、アウトカム、インパクトは、世界で私たちが観察するものなど、いくつかの仮定を考慮に入れることが多いです。人々が抱える課題。彼らがそれについて不満を言うかどうかにかかわらず。人々が愛し、望むもの。これらのニーズは、私たちがものを作りサービスを創造するために使う技術についての理解と組み合わさって、イノベーションの種となります。人々が抱えていると知っている問題を、彼らが解決策として想像するもので解決することは一つのことです。真のイノベーションとは、彼らが持っていると知らなかったニーズを、彼らが想像もできなかった解決策で満たすことです。これが個人とビジネスの成功の本当の秘密です。

<!-- - **Activities** — Talking, meetings, preparing, coding, testing, reducing technical debt, cooperating, and prioritizing. These are the day-to-day actions teams perform. Activities can be controlled.
- **Outputs** — Results from a team's activities that can be directly produced and measured. Features, to-do lists, action plans, Increments, standards, and sometimes even bugs. Outputs are tangible and easy to measure, but often mistaken for success. They demonstrate feasibility, which can guide the selection of the next inputs. Outputs can be influenced.
- **Outcomes** — Measurable changes in customer (including but not limited to users, choosers, internal customers, and other stakeholders) behavior or desired experience — like saving time, enjoying more reliable services, or achieving a smoother journey. Outcomes reveal whether outputs actually made a difference. Outcomes can be anticipated but are not predictable because they are emergent and often serendipitous. Learning from Outcomes may inform Assumptions or Input.
- **Impact** — The long-term organizational effects: revenue growth, improved ROI, cost savings, reputation, or market share. This is what secures survival and long-term competitiveness. For not-for-profit organizations or government institutions, impact can be measured by observable changes, such as a safer, happier public or a cleaner, more sustainable environment. Impact can only be observed. And it takes a cumulative outcome change over time to really have an impact. The impact informs future assumptions. -->

- **活動** — 会話、ミーティング、準備、コーディング、テスト、技術的負債の削減、協力、優先順位付け。これらはチームが行う日々のアクションです。活動は制御できます。
- **アウトプット** — チームの活動から直接生み出され測定できる結果。機能、ToDoリスト、アクションプラン、インクリメント、標準、そして時にはバグも。アウトプットは具体的で測定しやすいですが、しばしば成功と誤解されます。それらは実現可能性を示し、次のインプットの選択をガイドできます。アウトプットは影響を与えることができます。
- **アウトカム** — 顧客（ユーザー、選択者、内部顧客、その他のステークホルダーを含むがこれに限定されない）の行動または望ましい体験における測定可能な変化—時間の節約、より信頼性の高いサービスの享受、よりスムーズなジャーニーの達成など。アウトカムはアウトプットが実際に違いをもたらしたかどうかを明らかにします。アウトカムは予期できますが、創発的でしばしば偶発的であるため予測可能ではありません。アウトカムからの学習は仮定やインプットに情報を提供できます。
- **インパクト** — 長期的な組織への影響：収益成長、ROIの改善、コスト削減、評判、市場シェア。これが生存と長期的な競争力を確保するものです。非営利組織や政府機関にとって、インパクトは、より安全で幸せな市民、よりクリーンで持続可能な環境などの観察可能な変化によって測定できます。インパクトは観察することしかできません。そして、本当にインパクトを持つには、時間をかけた累積的なアウトカムの変化が必要です。インパクトは将来の仮定に情報を提供します。

<!-- **Bakery Analogy.** The bakery wants to be recognized as having the best cake in town, therefore it bakes and sells cakes: assumptions (baker's skills, high-quality ingredients, sufficient demand), inputs (flour, milk, mixer, work hours, recipes) → activities (preparing ingredients, mixing, baking, glazing) → output (cake) → outcome (people enjoy it, go for seconds) → impact (loyal customers, profit, recognition as the cake place in town). Without impact and customer outcomes, the bakery might be busy baking but have shelves full of unpurchased, unenjoyed cakes, and ultimately not achieve the objective and possibly go bankrupt. -->

**ベーカリーのアナロジー。** ベーカリーは町で最高のケーキを持つ店として認められたいと思い、そのためケーキを焼いて販売します：仮定（パン職人のスキル、高品質の材料、十分な需要）、インプット（小麦粉、牛乳、ミキサー、労働時間、レシピ）→ 活動（材料の準備、混合、焼成、アイシング）→ アウトプット（ケーキ）→ アウトカム（人々がそれを楽しみ、おかわりをする）→ インパクト（常連客、利益、町のケーキ店としての認知）。インパクトと顧客アウトカムがなければ、ベーカリーは焼くことに忙しくても、棚には買われず楽しまれないケーキが並び、最終的に目的を達成できず破産する可能性があります。

<!-- In software, teams often stop at the cake. Features are released and labeled as successful. But unless users benefit and are satisfied, and unless the organization benefits, the work has little value. -->

ソフトウェアでは、チームはしばしばケーキで止まってしまいます。機能がリリースされ、成功とラベル付けされます。しかし、ユーザーが恩恵を受けて満足しなければ、そして組織が恩恵を受けなければ、その作業にはほとんど価値がありません。

<!-- This also explains why so many "digital transformations" fall short. Companies adopt agile practices, speed up delivery, and push out more features - yet business metrics remain flat. What's missing is the focus on **clear objectives (assumptions)**, **inputs, outcomes, and impacts**. Jeff Bezos was famously known to emphasize **inputs** because they are easier to control - such as building a great team with the right tools, skills, and work environment [^20]. The real shift comes when organizations move beyond a project‑operating‑model, which measures success by output, to a product-operating model, which measures success by what truly changes for customers and the business. -->

これはまた、なぜ多くの「デジタルトランスフォーメーション」が期待を下回るかを説明します。企業はアジャイルプラクティスを採用し、納品を加速し、より多くの機能を押し出します—しかしビジネス指標は横ばいのままです。欠けているのは**明確な目標（仮定）**、**インプット、アウトカム、インパクト**への注力です。Jeff Bezosは**インプット**を強調することで有名でした。なぜなら、適切なツール、スキル、職場環境を備えた素晴らしいチームを構築するなど、インプットは制御しやすいからです[^20]。本当の転換は、組織がアウトプットで成功を測定するプロジェクト運用モデルを超えて、顧客とビジネスにとって本当に何が変わるかで成功を測定するプロダクト運用モデルへ移行するときに起こります。

<!-- Be aware that outcomes and impacts are not automatically positive. A new feature might succeed in changing customer behavior, but not in the way the team intended. For example, a social media platform introduces autoplay videos. The intended outcome was that user engagement would rise immediately as people spent more time scrolling. However, the change also increased data usage, drained phone batteries, and frustrated users. Over time, complaints grew, and the app rating fell. User frustration and complaints are still outcomes, but negative ones. This causes failure demand, the opposite of value demand [^19]. -->

アウトカムとインパクトは自動的にポジティブではないことに注意してください。新機能は顧客の行動を変えることに成功するかもしれませんが、チームが意図した方法ではないかもしれません。例えば、ソーシャルメディアプラットフォームが自動再生動画を導入します。意図されたアウトカムは、人々がスクロールにより多くの時間を費やすにつれてユーザーエンゲージメントがすぐに上昇することでした。しかし、この変更はデータ使用量を増加させ、電話のバッテリーを消耗させ、ユーザーをいらだたせました。時間が経つにつれて、苦情が増え、アプリの評価は下がりました。ユーザーの不満と苦情もアウトカムですが、ネガティブなものです。これは価値需要の反対である失敗需要を引き起こします[^19]。

<!-- The same applies at the impact level. An aggressive growth strategy might increase revenue in the short term, but it can also damage brand reputation or create unsustainable technical debt. In these cases, the outcome is real, and the impact is measurable, but both are harmful to the organization's long-term health. -->

同じことがインパクトレベルにも当てはまります。積極的な成長戦略は短期的には収益を増加させるかもしれませんが、ブランドの評判を傷つけたり、持続不可能な技術的負債を生み出したりする可能性もあります。これらの場合、アウトカムは実在し、インパクトは測定可能ですが、両方とも組織の長期的な健全性に有害です。

<!-- A strong product focus based on a product‑operating‑model addresses trade-offs, tensions, and non-negotiables between short-term wins and long-term consequences. -->

プロダクト運用モデルに基づく強力なプロダクトフォーカスは、短期的な勝利と長期的な結果の間のトレードオフ、緊張、譲れない点に対処します。

<!-- Acknowledging that outcomes and impacts can be negative keeps teams honest. It is a reminder that success is not defined by change alone, but by desirable change, experience, and the organization's resilience. -->

アウトカムとインパクトがネガティブになりうることを認識することで、チームは誠実さを保ちます。成功は変化だけで定義されるのではなく、望ましい変化、体験、そして組織のレジリエンスによって定義されるという注意喚起です。

<!-- As Annie Duke says in her work on decision-making, decisions should be judged not only by the outcomes they produce, but also by the quality of the process that led to them [^7]. A poor decision can occasionally lead to a lucky win, while a sound decision may still result in a setback. However, organizations that consistently base decisions on a transparent process that combines sound reasoning, evidence, and even counterintuitive psycho-logic [^28] [^29] [^30] achieve a more durable impact [^27]. This allows for objective decision assessment and the resulting process. -->

Annie Dukeが意思決定に関する著作で述べているように、意思決定はそれらが生み出すアウトカムだけでなく、それらに至ったプロセスの質によっても判断されるべきです[^7]。悪い意思決定が時々幸運な勝利につながることがあり、一方で健全な意思決定が依然として挫折をもたらす可能性があります。しかし、健全な推論、エビデンス、そして直感に反するサイコロジック[^28] [^29] [^30]を組み合わせた透明なプロセスに一貫して基づいて意思決定を行う組織は、より持続的なインパクトを達成します[^27]。これにより、客観的な意思決定評価と結果としてのプロセスが可能になります。

<!-- Outcomes and subsequent impacts have always been there. But shifting to a product operating model makes them visible and brings them into focus. When a Scrum Team focuses on them, it allows the team to really own and be accountable for what they create, their product. -->

アウトカムとそれに続くインパクトは常に存在してきました。しかし、プロダクト運用モデルへの移行により、それらが可視化され、焦点が当たるようになります。スクラムチームがそれらに注力すると、チームが自分たちが創造するもの、つまりプロダクトを本当に所有し、説明責任を持つことができるようになります。

<!-- At work, you may ask the following questions: -->

職場では、以下の質問をすることができます：

<!-- - What customer behavior should change, what might be directly observed? → **the customer outcomes and signals**
- How can the achievement of the outcome be verified? → **the product measures and signals**
- How can the achievement of the desired impact be verified?? → **the company measures and signals**
- What colleague behavior should change, what might be directly observed? → **the work climate outcomes and signals**
- What system behavior should change, what might be directly observed? → **the system of work outcomes and signals** -->

- どの顧客の行動が変わるべきで、何が直接観察できるか？ → **顧客アウトカムとシグナル**
- アウトカムの達成をどのように検証できるか？ → **プロダクトの指標とシグナル**
- 望ましいインパクトの達成をどのように検証できるか？ → **会社の指標とシグナル**
- どの同僚の行動が変わるべきで、何が直接観察できるか？ → **職場環境のアウトカムとシグナル**
- どのシステムの行動が変わるべきで、何が直接観察できるか？ → **仕事システムのアウトカムとシグナル**

<!-- ### From Output to Outcome -->

### アウトプットからアウトカムへ {#from-output-to-outcome}

<!-- The Scrum Guide Expansion Pack (SGEP) [^14] sharpens this distinction. It introduces the concepts of **Definition of Output Done** and **Definition of Outcome Done**. -->

Scrum Guide Expansion Pack（SGEP）[^14]はこの区別を明確にします。**アウトプット完成の定義**と**アウトカム完成の定義**の概念を導入しています。

<!-- - The **Definition of Output Done** ensures that the Increments the Scrum Team creates meet quality standards — good engineering practices, testing, documentation, security (and other non‑functional requirements), compliance & regulations, etc.
- The **Definition of Outcome Done** goes further. It asks whether the released Product achieved the intended customer change and business result. Only when outcomes are validated to a sufficient degree to support a decision can the work be considered truly "done." For example: In what ways was customer anxiety about the product's security reduced? How was the product's market position strengthened? How has the market share increased? Or, back to the bakery, did our customer pick up their cake, serve it at a party, see all their guests enjoy it, and then tell a few friends to go to the bakery? That's outcome done. -->

- **アウトプット完成の定義**は、スクラムチームが作成するインクリメントが品質基準を満たすことを保証します—良いエンジニアリングプラクティス、テスト、ドキュメント、セキュリティ（およびその他の非機能要件）、コンプライアンスと規制など。
- **アウトカム完成の定義**はさらに進みます。リリースされたプロダクトが意図した顧客の変化とビジネス結果を達成したかを問います。アウトカムが意思決定を支持するのに十分な程度まで検証されて初めて、作業は本当に「完成」と見なされます。例えば：プロダクトのセキュリティについての顧客の不安はどのような形で軽減されたか？プロダクトの市場ポジションはどのように強化されたか？市場シェアはどのように増加したか？あるいは、ベーカリーに戻ると、顧客はケーキを受け取り、パーティーで提供し、すべてのゲストがそれを楽しむのを見て、そして何人かの友人にベーカリーに行くよう伝えましたか？それがアウトカム完成です。

<!-- The focus on **outcome done** moves **impact** into the spotlight. Without organizational impact — growth, sustainability, resilience — there is no long-term success. Companies may run many Scrum Teams, deploy dozens of features, and still fail in the market if impacts are absent. A major global phone provider's decline is a classic example: outputs kept coming (great phones), but customer outcomes declined (nobody wanted them anymore), and the business impact turned negative. -->

**アウトカム完成**への注力は、**インパクト**をスポットライトに押し上げます。組織的なインパクト—成長、持続可能性、レジリエンス—がなければ、長期的な成功はありません。企業は多くのスクラムチームを運営し、数十の機能をデプロイしても、インパクトがなければ市場で失敗する可能性があります。ある大手グローバル携帯電話プロバイダーの衰退は典型的な例です：アウトプットは出続けました（素晴らしい電話）が、顧客アウトカムは低下し（誰もそれを望まなくなった）、ビジネスインパクトはネガティブになりました。

<!-- **Outcome‑focused Scrum** means: -->

**アウトカム重視のスクラム**とは：

<!-- - Scrum Teams are not just builders; they are **stewards or even explorers of value**.
- Product Owners are not Product Backlog secretaries; they are **strategic leaders ((SGEP/Strategy))**.
- Leaders are not **funders of projects**; they are **investors in outcomes** and, ultimately, in product impact.
- When evidence of value realization likelihood is not convincing, they gather quantitative and qualitative evidence on whether features are worth building (e.g., vibe coding, discovery research, customer discovery), but they are aware that the best feedback is result feedback when outputs are released and enabled. -->

- スクラムチームは単なる構築者ではなく、**価値のスチュワードまたは探検家**です。
- プロダクトオーナーはプロダクトバックログの秘書ではなく、**戦略的リーダー（(SGEP/Strategy)）**です。
- リーダーは**プロジェクトの資金提供者**ではなく、**アウトカムへの投資家**であり、最終的にはプロダクトインパクトへの投資家です。
- 価値実現の可能性についてのエビデンスが説得力を持たない場合、機能を構築する価値があるかどうかについて定量的・定性的エビデンスを収集します（例：バイブコーディング、ディスカバリーリサーチ、顧客発見）が、最良のフィードバックはアウトプットがリリースされ有効化されたときの結果フィードバックであることを認識しています。

<!-- This is what turns Scrum Teams into true committed, even missionary teams - driven by a direction of travel, accountable for outcomes, and committed to long-term impact. -->

これが、スクラムチームを真にコミットした、さらにはミッショナリーチームに変えるものです—進む方向によって駆動され、アウトカムに説明責任を持ち、長期的なインパクトにコミットしています。

<!-- ### The Learning Loop – Linking Work to Value -->

### 学習ループ – 作業を価値に結びつける {#the-learning-loop-linking-work-to-value}

<!-- A product's journey can also be understood through the (adapted) PDSA cycle (Plan–Do–Study–Act), a learning loop described by W. Edward Deming [^26]: -->

プロダクトの旅は（適応された）PDSAサイクル（Plan–Do–Study–Act）を通じても理解できます。これはW. Edward Demingによって説明された学習ループです[^26]：

<!-- - **Plan**: Based on stakeholder insights, the team hypothesizes (or has a hunch) that customers want a faster checkout. Research shows a high drop-off rate during payment entry, so the goal is to reduce cart abandonment from 42% to 30% within 2 Sprints.
- **Do**: The team prototypes and delivers a one-click checkout option with saved carts, ensuring compliance and good UX practices.
- **Study**: Telemetry data from A/B-tests shows time-to-purchase has been reduced from 5 minutes to 2 minutes, and Sprint Review feedback confirms positive customer reactions.
- **Act**: The team decides to continue improving the feature, rolling it out more widely while planning the next experiment based on what was learned. -->

- **Plan（計画）**: ステークホルダーの洞察に基づいて、チームは顧客がより速いチェックアウトを望んでいると仮説を立てます（または直感を持ちます）。調査は支払い入力時の高い離脱率を示しているため、目標は2スプリント以内にカート放棄率を42%から30%に削減することです。
- **Do（実行）**: チームはワンクリックチェックアウトオプションと保存されたカートをプロトタイプ化して提供し、コンプライアンスと良いUXプラクティスを確保します。
- **Study（研究）**: A/Bテストからのテレメトリデータは、購入までの時間が5分から2分に短縮されたことを示し、スプリントレビューのフィードバックは顧客の肯定的な反応を確認しています。
- **Act（改善）**: チームは機能の改善を続けることを決定し、学んだことに基づいて次の実験を計画しながら、より広範囲に展開します。

<!-- Seen this way, each Product Goal, Sprint Goal, or feature works like its own PDSA cycle — small learning loops that can occur at different levels or run in parallel. -->

このように見ると、各プロダクトゴール、スプリントゴール、または機能は独自のPDSAサイクルのように機能します—異なるレベルで発生したり、並行して実行できる小さな学習ループです。

<!-- Story maps also support this learning loop: they let teams choose a thin "first slice" of the journey (a walking skeleton) and then iteratively add depth based on evidence and feedback. [^21] -->

ストーリーマップもこの学習ループをサポートします：チームがジャーニーの薄い「最初のスライス」（ウォーキングスケルトン）を選び、その後エビデンスとフィードバックに基づいて反復的に深さを追加できるようにします。[^21]

<!-- To make this direction visible and discussable, many organizations use a Product Roadmap as an evolving communication tool that links goals, options, and decision points over time. Roadmaps are important, but this document treats them as their own topic, so they will be explained in a separate SGEP document rather than here. -->

この方向性を可視化し議論可能にするために、多くの組織はプロダクトロードマップを、目標、オプション、意思決定ポイントを時間軸で結びつける進化するコミュニケーションツールとして使用しています。ロードマップは重要ですが、この文書ではそれ自体をトピックとして扱っているため、ここではなく別のSGEP文書で説明されます。

<!-- Continuously. For more on (adapted PDSA), see the Planguage and Value Planning document. For more on strategy, see the strategy document ((SGEP/strategy)). -->

継続的に。（適応された）PDSAについての詳細は、PlanguageとValue Planningの文書を参照してください。戦略についての詳細は、戦略文書（(SGEP/strategy)）を参照してください。

<!-- ### Meaningful Checks per Sprint (keeping it real) -->

### スプリントごとの意味のあるチェック（現実を見据えて） {#meaningful-checks-per-sprint-keeping-it-real}

<!-- To ensure feasibility ("can it be built?") while reducing risk, Scrum Teams integrate small but powerful checks into each Sprint. These prevent wasted effort on ideas that look good in theory but collapse in practice. -->

フィージビリティ（「それは構築できるか？」）を確保しながらリスクを軽減するために、スクラムチームは各スプリントに小さいが強力なチェックを統合します。これらは、理論上は良く見えるが実際には崩壊するアイデアへの無駄な努力を防ぎます。

<!-- Here are a few ideas to consider when evaluating a Sprint. There is no need to cover all of them every Sprint: -->

スプリントを評価する際に検討すべきいくつかのアイデアがあります。毎スプリントすべてをカバーする必要はありません：

<!-- - **Spikes & technical prototypes as part of value delivery Product Backlog items**: Short, time-boxed investigations to explore unknowns early. -->

- **価値提供プロダクトバックログアイテムの一部としてのスパイクと技術プロトタイプ**: 未知のものを早期に探索するための短いタイムボックス化された調査。

<!--   _Example_: Before committing to a new recommendation engine, a team runs a timeboxed spike to compare tools or technologies based on model performance. -->

  _例_: 新しいレコメンデーションエンジンにコミットする前に、チームはモデルのパフォーマンスに基づいてツールや技術を比較するためにタイムボックス化されたスパイクを実行します。

<!-- - **Skill and capacity review**: Ask whether the team has the right people, skills, tools, and time for the proposed work. -->

- **スキルとキャパシティのレビュー**: チームが提案された作業に対して適切な人材、スキル、ツール、時間を持っているかを確認します。

<!--   _Example_: If a Sprint Backlog includes migrating to a new tool, but the team has no experience with containerization, feasibility declines unless training or external support is secured. -->

  _例_: スプリントバックログに新しいツールへの移行が含まれているが、チームにコンテナ化の経験がない場合、トレーニングや外部サポートが確保されない限り、フィージビリティは低下します。

<!-- - **Dependency mapping and breaking** (internal and external): Identify and make transparent any blockers across teams, vendors, or systems. Remove if possible. -->

- **依存関係のマッピングと解消**（内部および外部）: チーム、ベンダー、またはシステム間のブロッカーを特定し透明化します。可能であれば除去します。

<!--   _Example_: The checkout feature depends on a payment service from another company that only updates every few months. If the team doesn't spot this dependency early, it could delay the Sprint Goal. -->

  _例_: チェックアウト機能は、数ヶ月ごとにしか更新されない別の会社の決済サービスに依存しています。チームがこの依存関係を早期に発見しなければ、スプリントゴールが遅れる可能性があります。

<!-- - **Risk-based extensions**: Extend quality checks to match identified risks. -->

- **リスクベースの拡張**: 特定されたリスクに合わせて品質チェックを拡張します。

<!--   _Example_: For a high-traffic e-commerce site, the acceptance criteria might include "checkout response time < 2 seconds on staging with 1,000 concurrent users." Performance and scalability risks are handled before release, not after. Ideally, addressed with the Definition of Output Done. -->

  _例_: 高トラフィックのeコマースサイトの場合、受け入れ基準には「ステージング環境で1,000の同時ユーザーでチェックアウト応答時間 < 2秒」が含まれる可能性があります。パフォーマンスとスケーラビリティのリスクはリリース後ではなく、リリース前に対処されます。理想的には、アウトプット完成の定義で対処されます。

<!-- - **Go/No-Go experiment criteria before continuing**: Define simple success/failure signals for an idea before investing heavily. -->

- **続行前のGo/No-Go実験基準**: 大きな投資をする前に、アイデアの簡単な成功/失敗シグナルを定義します。

<!--   _Example_: A landing page prototype is tested with 200 real customers. Criteria: at least 15% sign-up conversion rate, and 60% of customers got motivated for learning. If this 'kill-criteria' is not met, the team pivots before building the full feature. Addressed with the Definition of Outcome Done. -->

  _例_: ランディングページのプロトタイプを200人の実顧客でテストします。基準：少なくとも15%のサインアップコンバージョン率、60%の顧客が学習に動機付けられること。この「中止基準」が満たされない場合、チームはフル機能を構築する前にピボットします。アウトカム完成の定義で対処されます。

<!-- - **Desirability check or product telemetry analysis (user motivation and love):** Validate whether the solution resonates with users, not just whether it solves a problem. -->

- **魅力性チェックまたはプロダクトテレメトリ分析（ユーザーの動機と愛着）:** ソリューションが問題を解決するかだけでなく、ユーザーに共感されるかを検証します。

<!--   _Example:_ Before finalizing a new dashboard layout, the team tests whether users find it clearer and more engaging, not just functional. Low emotional engagement signals risk of disuse. -->

  _例_: 新しいダッシュボードレイアウトを確定する前に、チームはユーザーがそれを単に機能的であるだけでなく、より明確で魅力的と感じるかをテストします。低い感情的エンゲージメントは使われなくなるリスクを示唆します。

<!-- - **Viability check (sustainability):** Ensure the solution makes business sense in practice, e.g., within the business constraints. -->

- **実現可能性チェック（持続可能性）:** ソリューションがビジネス上の制約内で実際にビジネス的に意味があることを確認します。

<!--   _Example:_ A new AI feature is promising, but legal reviews and infrastructure costs reveal it is not viable within the current budget or compliance environment. Adjustments are made before development. -->

  _例_: 新しいAI機能は有望ですが、法的レビューとインフラコストにより、現在の予算やコンプライアンス環境内では実現可能ではないことが明らかになります。開発前に調整が行われます。

<!-- - **Continuous compliance feasibility**: In regulated industries, add (ideally automated) fulfillment checks around rules and standards. -->

- **継続的コンプライアンスのフィージビリティ**: 規制産業では、ルールと標準に関する（理想的には自動化された）遵守チェックを追加します。

<!--   _Example_: A health app feature is tested for GDPR and HIPAA compliance during the prototype stage or at every Sprint, preventing costly redesigns later. Addressed with the Definition of Output Done. -->

  _例_: ヘルスアプリの機能は、プロトタイプ段階または各スプリントでGDPRとHIPAAのコンプライアンスがテストされ、後のコストのかかる再設計を防ぎます。アウトプット完成の定義で対処されます。

<!-- - **Tooling and infrastructure validation**: Ensure environments, test data, and deployment pipelines are in place to support the work. -->

- **ツールとインフラの検証**: 環境、テストデータ、デプロイメントパイプラインが作業をサポートするために整っていることを確認します。

<!--   _Example_: Before committing to an AI-powered search, the team verifies that anonymized training data is available and legally permissible for use. -->

  _例_: AIを活用した検索にコミットする前に、チームは匿名化されたトレーニングデータが利用可能で法的に使用が許可されていることを確認します。

<!-- ## Missionary vs. Mercenary Teams -->

## ミッショナリーチーム vs. マーセナリーチーム {#missionary-vs-mercenary-teams}

<!-- Marty Cagan and John Doerr popularized the distinction between missionary and mercenary teams [^8]. It is a powerful metaphor for understanding the required cultural shift. -->

Marty CaganとJohn Doerrはミッショナリーチームとマーセナリーチームの区別を広めました[^8]。これは必要な文化的転換を理解するための強力なメタファーです。

<!-- **Mercenary teams** deliver what they are told to do. They are professional, competent, and focused on execution. But they do not own the outcome. Their job ends with delivering output. They have a delivery mindset. -->

**マーセナリーチーム**は言われたことを納品します。彼らはプロフェッショナルで、有能で、実行に集中しています。しかし、彼らはアウトカムを所有しません。彼らの仕事はアウトプットを納品することで終わります。彼らはデリバリーマインドセットを持っています。

<!-- **Missionary teams** care deeply about the problem they are solving. They are committed to the product strategy, not just the tasks. They own the full value stream - from assumptions, inputs, and activities through outputs to outcomes and impacts. They constantly ask: Did life improve for the customer? How do we know? Did the needle move for the business? How do we know? They follow a value-oriented mode of operation. And, like missionaries in the real world, they're not always successful. They endure a lot of hardship. But do so because ultimately, having an impact is more important to them than their short-term gains. -->

**ミッショナリーチーム**は解決しようとしている問題に深く関心を持っています。彼らはタスクだけでなく、プロダクト戦略にコミットしています。彼らは仮定、インプット、活動からアウトプット、アウトカム、インパクトまでの完全なバリューストリームを所有しています。彼らは常に問います：顧客の生活は改善したか？どうやって分かるのか？ビジネスの針は動いたか？どうやって分かるのか？彼らは価値志向の運用モードに従います。そして、現実世界の宣教師のように、彼らは常に成功するわけではありません。彼らは多くの困難に耐えます。しかし、そうするのは最終的に、インパクトを持つことが短期的な利益よりも彼らにとって重要だからです。

<!-- Neither metaphor should be taken too literally. Mercenaries are not "bad," and missionaries are not "perfect." But the distinction helps see the kind of ownership and passion required in modern product teams. -->

どちらのメタファーも文字通りに取りすぎるべきではありません。マーセナリーは「悪い」わけではなく、ミッショナリーは「完璧」ではありません。しかし、この区別は現代のプロダクトチームに必要なオーナーシップと情熱の種類を見るのに役立ちます。

<!-- From a strategic perspective, mercenary teams are paid to deliver outputs, typically without worrying whether those outputs create meaningful impact. Missionary teams, by contrast, link daily work to strategic outcomes. They embody an emergent, continuous adaptive strategy: constantly adjusting to market signals and ensuring the company's long-term impact remains positive. -->

戦略的な観点から、マーセナリーチームはアウトプットを納品するために報酬を得ており、通常、それらのアウトプットが意味のあるインパクトを生み出すかどうかを心配しません。対照的に、ミッショナリーチームは日々の作業を戦略的アウトカムに結びつけます。彼らは創発的で継続的な適応戦略を体現しています：市場シグナルに絶えず調整し、会社の長期的なインパクトがポジティブであり続けることを確保します。

<!-- Either a mercenary or missionary team might say: "We built the feature as specified."
 or "We improved customer happiness by saving 50% of their time, checkout speed by 30%, which led to 15% more completed purchases." But a missionary team might also ask after a Product release: "Where is the evidence that enough desired outcomes were achieved?" or "What do we need to do to really achieve enough of the desired outcomes? Where can we improve?" -->

マーセナリーチームでもミッショナリーチームでも「仕様通りに機能を構築しました」と言うかもしれません。または「顧客の時間を50%節約し、チェックアウト速度を30%改善することで顧客の幸福度を向上させ、それにより購入完了が15%増加しました」と言うかもしれません。しかし、ミッショナリーチームはプロダクトリリース後に「望ましいアウトカムが十分に達成されたというエビデンスはどこにあるのか？」や「望ましいアウトカムを本当に十分に達成するために何をする必要があるのか？どこを改善できるのか？」と問うこともあります。

<!-- The difference is profound. One team measures success in output. The other measures success based on outcomes and impact. -->

その違いは深遠です。一方のチームはアウトプットで成功を測定します。もう一方はアウトカムとインパクトに基づいて成功を測定します。

<!-- This is precisely the stance effective Product Owners take: they frame work as hypotheses tied to value or problems to be solved and steer toward outcomes, not activity [^18]. -->

これはまさに効果的なプロダクトオーナーが取るスタンスです：彼らは作業を価値に結びついた仮説または解決すべき問題としてフレーミングし、活動ではなくアウトカムに向けて舵を取ります[^18]。

<!-- Missionary teams also have a sharper eye on the competition. They are not content to satisfy only internal stakeholders; they monitor the market, compare experiences, and ask: _If competitors released the same feature tomorrow, would the product still stand out?_ By linking their **why** to both customer needs and competitive positioning, they ensure their work creates defensible impact rather than fleeting output [^9]. -->

ミッショナリーチームはまた競争に対してより鋭い目を持っています。彼らは内部のステークホルダーだけを満足させることに満足しません。彼らは市場を監視し、体験を比較し、問います：_競合他社が明日同じ機能をリリースしたら、このプロダクトはまだ際立っているだろうか？_ 彼らの**なぜ**を顧客のニーズと競争上のポジショニングの両方に結びつけることで、彼らの作業が一時的なアウトプットではなく防御可能なインパクトを生み出すことを確保します[^9]。

<!-- Good Scrum Teams act as missionary teams. -->

良いスクラムチームはミッショナリーチームとして行動します。

<!-- ## Evidence-Based Management (EBM) -->

## エビデンスベースドマネジメント（EBM） {#evidence-based-management-ebm}

<!-- How are outcomes and impacts measured in practice? This is where Evidence-Based Management (EBM) comes in. Developed by Scrum.org, EBM [^5] provides a framework for managing and improving value delivery. -->

アウトカムとインパクトは実際にはどのように測定されるのでしょうか？ここでEvidence-Based Management（EBM）が登場します。Scrum.orgによって開発されたEBM[^5]は、価値提供を管理し改善するためのフレームワークを提供します。

<!-- EBM rests on four Key Value Areas (KVAs): -->

EBMは4つの重要価値領域（KVA）に基づいています：

<!-- - **Current Value (CV):** How much value are customers, users, and the organization receiving today?
- **Unrealized Value (UV):** How much potential value is still out there?
- **Ability to Innovate (A2I):** How capable is the organization of improving and adapting?
- **Time to Market (T2M):** How quickly can new value be delivered? -->

- **現在価値（CV）:** 顧客、ユーザー、組織は今日どれだけの価値を受け取っているか？
- **未実現価値（UV）:** まだどれだけの潜在的価値が残っているか？
- **イノベーション能力（A2I）:** 組織は改善と適応にどれだけ能力があるか？
- **市場投入時間（T2M）:** 新しい価値をどれだけ迅速に提供できるか？

<!-- Together, these areas encourage teams to look beyond velocity or throughput (merely activity/output measures, often referred to as vanity metrics). Instead, they link organizational capabilities (A2I and T2M) to market value (CV and UV) through a balanced set of measures that provide a signal via telemetry. -->

これらの領域は合わせて、チームがベロシティやスループット（単なる活動/アウトプット指標、しばしばバニティメトリクスと呼ばれる）を超えて見ることを奨励します。代わりに、テレメトリを通じてシグナルを提供するバランスの取れた指標セットを通じて、組織の能力（A2IとT2M）を市場価値（CVとUV）に結びつけます。

<!-- In strategic terms, EBM serves as a feedback loop informing the relationship between strategy deployment and emergent strategy. Traditionally, strategy deployment pushes objectives down the hierarchy: leadership sets impact goals, and teams are tasked with delivering outputs that, ideally, align. Emergent strategy, on the other hand, allows teams to discover outcomes through experimentation, observation, and more, and roll those insights up into the strategy. EBM helps leaders validate whether strategic bets are translating into real impact, while empowering teams to adapt locally [^10]. -->

戦略的な観点から、EBMは戦略展開と創発戦略の関係に情報を提供するフィードバックループとして機能します。従来、戦略展開は目標を階層の下に押し下げます：リーダーシップがインパクト目標を設定し、チームは理想的には整合するアウトプットを提供する任務を与えられます。一方、創発戦略はチームが実験、観察などを通じてアウトカムを発見し、それらの洞察を戦略に組み込むことを可能にします。EBMはリーダーが戦略的な賭けが実際のインパクトに変換されているかを検証するのを助け、同時にチームがローカルで適応することを可能にします[^10]。

<!-- EBM also encourages a shift from circumstantial leading indicators to lagging direct evidence - and highlights the role of assumptions and **inputs** in shaping both. -->

EBMはまた、状況的な先行指標から遅行する直接的エビデンスへの転換を奨励し、両方を形作る上での仮定と**インプット**の役割を強調します。

<!-- - A **Goal** is the assumption of an objective to be achieved. It is not yet known whether this is feasible or valuable. -->

- **ゴール**は達成すべき目標の仮定です。これが実現可能か価値があるかはまだ分かりません。

<!-- - **Leading indicators** are early signals that inputs and outputs are moving in the right direction—such as higher release frequency after investing in CI/CD or faster experiment cycles after adding UX research. Because they show up quickly, they're useful for adjusting course as conditions change. Also, leading indicators are early signals that outcomes are moving in the right direction. -->

- **先行指標**は、インプットとアウトプットが正しい方向に動いているという早期シグナルです—CI/CDへの投資後のリリース頻度の向上や、UXリサーチ追加後の実験サイクルの高速化など。それらはすぐに現れるため、状況が変化する際にコースを調整するのに役立ちます。また、先行指標はアウトカムが正しい方向に動いているという早期シグナルでもあります。

<!-- - **Lagging indicators** confirm (or not) whether those earlier signals turned into real (delayed) outcomes and subsequent impact - like active-user growth, lower churn, or better ROI. They appear later, giving hard evidence of whether the decisions actually worked. -->

- **遅行指標**は、それらの初期シグナルが実際の（遅延した）アウトカムとその後のインパクトになったかどうかを確認します（または確認しません）—アクティブユーザーの成長、離脱率の低下、ROIの改善など。それらは後で現れ、意思決定が実際に機能したかどうかの確かなエビデンスを提供します。

<!-- By combining experiments with **input tracking, leading signals, and lagging evidence**, teams can validate whether their efforts are producing outputs, creating outcomes, and generating impacts. This creates a continuous learning environment where inputs are actively adjusted, signals inspected, and impacts measured. -->

実験と**インプット追跡、先行シグナル、遅行エビデンス**を組み合わせることで、チームは自分たちの努力がアウトプットを生み出し、アウトカムを創造し、インパクトを生成しているかどうかを検証できます。これにより、インプットが積極的に調整され、シグナルが検査され、インパクトが測定される継続的な学習環境が作られます。

<!-- Here too, the **why** for **whom** matters. Evidence without purpose is just data. The strategic role of EBM is to anchor metrics — from inputs through outcomes — to the organization's larger **why**: its vision, its customers, and its competitive context. Without that anchor, teams risk chasing numbers that look good in dashboards but do not strengthen the company's long-term impact. -->

ここでも、**誰のために**の**なぜ**が重要です。目的のないエビデンスは単なるデータです。EBMの戦略的役割は、指標を—インプットからアウトカムまで—組織のより大きな**なぜ**に固定することです：そのビジョン、顧客、競争的文脈。その固定がなければ、チームはダッシュボードでは良く見えるが会社の長期的インパクトを強化しない数字を追いかけるリスクがあります。

<!-- EBM also relies on clearly stated goals across different horizons—strategic, intermediate, and tactical. These goals provide the context that links evidence to purpose, helping Scrum Teams and leaders decide not just what is happening with the product today, but whether they are moving the product closer to delivering the outcomes and impacts that matter most. -->

EBMはまた、戦略的、中間的、戦術的という異なる視野にまたがる明確に述べられたゴールに依存しています。これらのゴールはエビデンスを目的に結びつける文脈を提供し、スクラムチームとリーダーが今日プロダクトで何が起こっているかだけでなく、最も重要なアウトカムとインパクトを提供することにプロダクトを近づけているかどうかを判断するのを助けます。

<!-- ## Data Collection and Decision Making -->

## データ収集と意思決定 {#data-collection-and-decision-making}

<!-- A clear measurement framework helps, but raw **data** is also required. Modern product teams are fortunate to operate in a digital environment where telemetry, the automated collection of usage data, provides a near real-time view of how products are used. -->

明確な測定フレームワークは役立ちますが、生の**データ**も必要です。現代のプロダクトチームは、テレメトリ（使用データの自動収集）がプロダクトの使用方法をほぼリアルタイムで表示するデジタル環境で運用できることは幸運です。

<!-- **Telemetry [^24] answers critical questions, and the questions will depend on the context. Here is a list of examples:** -->

**テレメトリ[^24]は重要な質問に答え、質問は文脈に依存します。以下は例のリストです：**

<!-- **1. Usage & Adoption** -->

**1. 使用とアダプション**

<!-- - Which features are used, by whom, and which are never used?
- How frequently are key features used?
- Which user groups behave differently? -->

- どの機能が、誰によって使用され、どの機能は全く使用されていないか？
- 主要機能はどれくらいの頻度で使用されているか？
- どのユーザーグループが異なる行動をしているか？

<!-- **2. Engagement & Retention** -->

**2. エンゲージメントとリテンション**

<!-- - How often do users return (daily, weekly, monthly)?
- How long do users stay active before dropping off?
- What actions predict long-term use? -->

- ユーザーはどれくらいの頻度で戻ってくるか（毎日、毎週、毎月）？
- ユーザーは離脱するまでどれくらいアクティブでいるか？
- どのアクションが長期使用を予測するか？

<!-- **3. Flow & Friction (deeper than abandonment)** -->

**3. フローとフリクション（離脱よりも深く）**

<!-- - Where do users hesitate, retry, or slow down?
- Which steps cause the most errors or retries?
- Where do users need help or support? -->

- ユーザーはどこでためらい、リトライし、速度を落とすか？
- どのステップが最も多くのエラーやリトライを引き起こすか？
- ユーザーはどこでヘルプやサポートを必要とするか？

<!-- **4. Value Realization** -->

**4. 価値実現**

<!-- - Do users reach the intended outcome?
- How long does it take users to get value for the first time?
- Which behaviors correlate with success? -->

- ユーザーは意図されたアウトカムに到達しているか？
- ユーザーが初めて価値を得るまでにどれくらいかかるか？
- どの行動が成功と相関しているか？

<!-- **5. Change Over Time** -->

**5. 時間の経過による変化**

<!-- - How does behavior change after a release?
- Did a new feature replace an old workaround?
- Are users adapting or ignoring the change? -->

- リリース後に行動はどのように変化するか？
- 新機能は古い回避策を置き換えたか？
- ユーザーは変更に適応しているか、無視しているか？

<!-- **6. Risk & Quality Signals** -->

**6. リスクと品質のシグナル**

<!-- - Which actions lead to crashes, errors, or support tickets?
- Are there patterns before churn or complaints?
- Which users are at risk of leaving? -->

- どのアクションがクラッシュ、エラー、サポートチケットにつながるか？
- 離脱や苦情の前にパターンがあるか？
- どのユーザーが離脱リスクがあるか？

<!-- **7. Business-Relevant Signals** -->

**7. ビジネス関連シグナル**

<!-- - Which behaviors correlate with upgrades or renewals?
- Which features are used by high-value customers?
- What usage patterns predict willingness to pay? -->

- どの行動がアップグレードや更新と相関しているか？
- 高価値顧客はどの機能を使用しているか？
- どの使用パターンが支払い意欲を予測するか？

<!-- This matters because not all signals are equally strong. A spike in page views might look promising, but if users abandon the flow before completing a task, the signal is weak. By contrast, sustained daily use, customer referrals, or willingness to pay are strong signals of value. -->

これが重要なのは、すべてのシグナルが等しく強力ではないからです。ページビューの急上昇は有望に見えるかもしれませんが、ユーザーがタスクを完了する前にフローを離脱した場合、そのシグナルは弱いです。対照的に、持続的な日次使用、顧客からの紹介、支払い意欲は価値の強力なシグナルです。

<!-- Retiring unused features is equally important. Every feature carries a maintenance cost. If telemetry shows little adoption, the courageous choice might be to retire it. This creates space for investing in outcomes that matter. -->

使用されていない機能の廃止も同様に重要です。すべての機能にはメンテナンスコストがかかります。テレメトリがほとんど採用されていないことを示している場合、勇気ある選択はそれを廃止することかもしれません。これにより、重要なアウトカムに投資する余地が生まれます。

<!-- Data collection alone does not create value. Teams must build a discipline of **data‑informed** decision-making and integrate it into their product‑operating‑model. That means decisions are guided by evidence, but not enslaved to it. Numbers lack context; teams bring purpose and vision to interpret what signals really mean. The **why** for the **whom** behind the data turns metrics into actionable insight. -->

データ収集だけでは価値は生まれません。チームは**データインフォームド**な意思決定の規律を構築し、それをプロダクト運用モデルに統合する必要があります。これは意思決定がエビデンスによって導かれるが、それに隷属しないことを意味します。数字には文脈がありません。チームはシグナルが実際に何を意味するかを解釈するために目的とビジョンを持ち込みます。データの背後にある**誰のために**の**なぜ**が指標を実行可能な洞察に変えます。

<!-- It is encouraged to use both quantitative data (e.g., number of active users, time to complete a task) and qualitative data (e.g., customer feedback, user interviews, or user observations). Together, they provide a fuller picture: the numbers show **what** is happening, while stories and observations explain **why**. -->

定量的データ（例：アクティブユーザー数、タスク完了までの時間）と定性的データ（例：顧客フィードバック、ユーザーインタビュー、ユーザー観察）の両方を使用することが推奨されます。それらを合わせると、より完全な絵が提供されます：数字は**何が**起こっているかを示し、ストーリーと観察は**なぜ**を説明します。

<!-- ## Making Decisions Informed by Evidence -->

## エビデンスに基づいた意思決定 {#making-decisions-informed-by-evidence}

<!-- Adaptation without facts is guesswork. Product management requires choices: which customers to prioritize, which bets to fund, which experiments to scale. -->

事実なしの適応は当て推量です。プロダクトマネジメントには選択が必要です：どの顧客を優先するか、どの賭けに資金を提供するか、どの実験を拡大するか。

<!-- Evidence-informed decision-making closes the gap between intuition and reality. It does not mean eliminating judgment; it means grounding judgment in evidence. Be open to psycho-logic: the opposite of a good idea might be another good idea [^28]; if every idea is rational, the competition will do the same things. A Product Owner deciding which feature to invest in might ask: -->

エビデンスインフォームドな意思決定は、直感と現実の間のギャップを埋めます。それは判断を排除することを意味しません。判断をエビデンスに根拠付けることを意味します。サイコロジックに対してオープンでいてください：良いアイデアの反対は別の良いアイデアかもしれません[^28]。すべてのアイデアが合理的であれば、競合他社も同じことをするでしょう。どの機能に投資するかを決定するプロダクトオーナーは次のように問うかもしれません：

<!-- - What data supports this choice?
- What assumptions are being made?
- How will success be known?
- Which experiment could validate the assumption?
- What critical thinking has been applied? -->

- この選択を支持するデータは何か？
- どのような仮定がなされているか？
- 成功をどのように知ることができるか？
- どの実験が仮定を検証できるか？
- どのようなクリティカルシンキングが適用されたか？

<!-- The discipline is simple but powerful: **state assumptions or hunches, collect evidence, inspect results, and adapt**. This creates a feedback loop that replaces opinion-driven debates with learning-driven action. Leaders, especially Supporters [^14], have a role too: rather than rewarding certainty, they must create a safe environment for admitting uncertainty and adjusting based on facts. -->

その規律はシンプルだが強力です：**仮定や直感を述べ、エビデンスを収集し、結果を検査し、適応する**。これは意見駆動の議論を学習駆動のアクションで置き換えるフィードバックループを作ります。リーダー、特にサポーター[^14]にも役割があります：確実性を報いるのではなく、不確実性を認め、事実に基づいて調整するための安全な環境を作らなければなりません。

<!-- Without this discipline, organizations fall into two popular traps (there could be more). One is **HiPPO decisions** [^15]— following the Highest Paid Person's Opinion. The other is **analysis paralysis** — drowning in dashboards without making choices. Fact-or-figure-informed decision-making strikes a balance: enough evidence to reduce risk and enough courage to act. It also helps Scrum Teams minimize cognitive and organizational biases that can distort judgment. -->

この規律がなければ、組織は2つの一般的な罠に陥ります（もっとあるかもしれません）。1つは**HiPPO決定**[^15]—最も給与の高い人の意見に従うこと。もう1つは**分析麻痺**—選択をせずにダッシュボードに溺れること。事実または数値に基づいた意思決定はバランスを取ります：リスクを軽減するのに十分なエビデンスと行動する十分な勇気。また、判断を歪める可能性のある認知的および組織的バイアスを最小化するのにスクラムチームを助けます。

<!-- One of the most useful ways to set goals is to identify value that likely exists but hasn't been captured yet. This means making educated guesses about where the biggest gaps are between what customers get today and what they still need. By comparing current customer outcomes with unmet needs (and what competitors offer), teams can spot the most promising opportunities. For example, if customers use the product frequently but repeatedly complain about a missing capability, that's a strong signal that the capability is worth pursuing. Used this way, these educated guesses help focus investment where the potential return is highest. Human decision-making is often based on emotions and biases - not necessarily always logical. While making a decision, these human traits should be recognized, even leveraged. -->

ゴールを設定する最も有用な方法の1つは、おそらく存在するがまだ捕捉されていない価値を特定することです。これは、顧客が今日得ているものとまだ必要としているものの間の最大のギャップがどこにあるかについて教育された推測をすることを意味します。現在の顧客アウトカムを満たされていないニーズ（および競合他社が提供するもの）と比較することで、チームは最も有望な機会を見つけることができます。例えば、顧客が製品を頻繁に使用しているが、欠けている機能について繰り返し不満を言っている場合、その機能は追求する価値があるという強力なシグナルです。このように使用すると、これらの教育された推測は、潜在的なリターンが最も高いところに投資を集中するのに役立ちます。人間の意思決定はしばしば感情とバイアスに基づいています—必ずしも常に論理的ではありません。意思決定を行う際、これらの人間的特性は認識され、さらには活用されるべきです。

<!-- ## Product Risk Management -->

## プロダクトリスクマネジメント {#product-risk-management}

<!-- Another reason that project‑operating‑models fail is a classical approach to risk management. Risk is often treated as something to eliminate with upfront analysis and control. But in complex domains, most risks cannot be fully known in advance. Risk is good when it is made visible early and used to guide learning. Agile approaches manage risk differently: by delivering in small Increments, proactively prioritizing risk reduction, testing assumptions early, and using feedback to correct course. Leveraging those as enabling constraints allows Scrum Teams to reduce uncertainty while still moving forward. Managing risk this way keeps organizations adaptive, prevents costly failures, and improves the chances that money, effort, and other resources are spent on what truly matters. This is an emergent strategy applied (also known as a continuous adaptive strategy). -->

プロジェクト運用モデルが失敗するもう1つの理由は、リスクマネジメントへの古典的なアプローチです。リスクはしばしば事前の分析とコントロールで排除すべきものとして扱われます。しかし、複雑なドメインでは、ほとんどのリスクは事前に完全に知ることができません。リスクは早期に可視化され、学習を導くために使用されるときは良いものです。アジャイルアプローチはリスクを異なる方法で管理します：小さなインクリメントで提供し、リスク削減を積極的に優先し、仮定を早期にテストし、フィードバックを使ってコースを修正します。それらを可能にする制約として活用することで、スクラムチームは前進しながら不確実性を減らすことができます。この方法でリスクを管理することで、組織は適応性を維持し、コストのかかる失敗を防ぎ、お金、努力、その他のリソースが本当に重要なものに費やされる可能性を高めます。これは適用された創発戦略です（継続的適応戦略としても知られています）。

<!-- An Agile approach to risk management has always involved: -->

リスクマネジメントへのアジャイルアプローチは常に以下を含んできました：

<!-- - **Small Increments:** Reducing exposure by releasing frequently.
- **Continuous discovery with early validation:** Build to learn with prototypes or experiments before scaling.
- **Feedback loops:** Using telemetry and customer feedback as continuous risk signals.
- **Portfolio thinking:** Diversifying bets (with "kill criteria") rather than putting all money and efforts into one initiative. -->

- **小さなインクリメント:** 頻繁にリリースすることで露出を減らす。
- **早期検証を伴う継続的発見:** スケールする前にプロトタイプや実験で学ぶために構築する。
- **フィードバックループ:** テレメトリと顧客フィードバックを継続的なリスクシグナルとして使用する。
- **ポートフォリオ思考:** すべてのお金と努力を1つのイニシアチブに投入するのではなく、賭けを分散する（「中止基準」付きで）。

<!-- The **why** here is 1). survival in uncertainty and 2). excelling in value improvement. By managing risk adaptively, organizations avoid the false comfort of static plans. They learn faster than competitors and adjust before risks become existential. In practice, this means risk registers and upfront mitigation plans are replaced with living experiments and **signal‑based evidence‑informed** decisions. -->

ここでの**なぜ**は1) 不確実性の中での生存と 2) 価値改善における卓越です。リスクを適応的に管理することで、組織は静的な計画の誤った安心感を避けます。競合他社よりも早く学び、リスクが存亡に関わる前に調整します。実際には、これはリスク登録簿と事前の軽減計画が、生きた実験と**シグナルベースのエビデンスインフォームド**な意思決定に置き換えられることを意味します。

<!-- Adaptive risk management turns uncertainty from a threat into an asset. Variation in outcomes is not feared - it is the source of learning that guides future strategy; it is a competitive advantage. -->

適応的リスクマネジメントは不確実性を脅威から資産に変えます。アウトカムのばらつきは恐れられません—それは将来の戦略を導く学習の源です。それは競争優位です。

<!-- ### Product Engineering Practices for Digital Products – Building for Feasibility and Risk Reduction -->

### デジタルプロダクトのためのプロダクトエンジニアリングプラクティス – フィージビリティとリスク削減のための構築 {#product-engineering-practices-for-digital-products-building-for-feasibility-and-risk-reduction}

<!-- In digital products, strong engineering practices reduce product risk and ensure feasibility: -->

デジタルプロダクトにおいて、強力なエンジニアリングプラクティスはプロダクトリスクを減らし、フィージビリティを確保します：

<!-- - **Test automation:** Using software tools to automatically run tests, check results, and report issues - making testing faster, repeatable, and more reliable
- **CI/CD pipelines:** Frequent integration and deployment reduce release risk.
- **Trunk‑based development:** Keeps work integrated, reducing merge conflicts.
- **Feature flags & canary releases:** Enable safe experimentation and gradual rollouts.
- **Observability (SLO/SLA/SI) [^25]:** Telemetry, error rates, and performance signals ensure quality **in use**.
- **Security by design:** Embedding security testing and compliance checks into the Definition of Output Done. -->

- **テスト自動化:** ソフトウェアツールを使用してテストを自動的に実行し、結果をチェックし、問題を報告する—テストをより速く、繰り返し可能で、より信頼性の高いものにする
- **CI/CDパイプライン:** 頻繁な統合とデプロイメントがリリースリスクを減らす。
- **トランクベース開発:** 作業を統合された状態に保ち、マージコンフリクトを減らす。
- **フィーチャーフラグとカナリアリリース:** 安全な実験と段階的なロールアウトを可能にする。
- **オブザーバビリティ（SLO/SLA/SI）[^25]:** テレメトリ、エラー率、パフォーマンスシグナルが**使用中の**品質を確保する。
- **セキュリティバイデザイン:** セキュリティテストとコンプライアンスチェックをアウトプット完成の定義に組み込む。

<!-- These practices tie engineering excellence ((SGEP/SoftwareEngineeringPractices)) directly to value delivery, turning quality into a risk‑reduction tool. Similar principles apply to non-IT products as well: in domains such as healthcare, medical devices, and pharmaceuticals, practices such as automated quality checks, small-batch experimentation, and regulatory compliance embedded early in the process serve the same purpose: reducing risk. -->

これらのプラクティスはエンジニアリングエクセレンス（(SGEP/SoftwareEngineeringPractices)）を価値提供に直接結びつけ、品質をリスク削減ツールに変えます。同様の原則は非ITプロダクトにも適用されます：医療、医療機器、製薬などのドメインでは、自動化された品質チェック、小バッチ実験、プロセスの早い段階に組み込まれた規制コンプライアンスなどのプラクティスが同じ目的を果たします：リスクを減らすこと。

<!-- ## Compliance and Regulations -->

## コンプライアンスと規制 {#compliance-and-regulations}

<!-- Compliance is often seen as an obstacle to agile product management. In regulated industries - finance, healthcare, energy - teams may assume they cannot be agile because every release must pass strict audits. But compliance and agility are not opposites. Done well, they reinforce each other. For example, change agents could foster regular, intentional collaboration between the product team and single points of contact to determine how each set of compliance risks would enable continuous compliance at pace. -->

コンプライアンスはしばしばアジャイルプロダクトマネジメントの障害として見られます。規制産業—金融、医療、エネルギー—では、すべてのリリースが厳格な監査を通過しなければならないため、チームはアジャイルになれないと仮定するかもしれません。しかし、コンプライアンスとアジリティは反対ではありません。うまく行えば、それらは互いを強化します。例えば、変革エージェントは、各コンプライアンスリスクのセットがペースに合った継続的コンプライアンスをどのように可能にするかを決定するために、プロダクトチームと単一の連絡窓口間の定期的で意図的なコラボレーションを促進できます。

<!-- The **Definition of Output Done** in the SGEP ensures that Increments meet the agreed quality standards. In regulated environments, these standards must include **compliance and regulatory checks**. A feature that works for customers but violates data privacy rules is not truly "output done." -->

SGEPの**アウトプット完成の定義**は、インクリメントが合意された品質基準を満たすことを保証します。規制環境では、これらの基準には**コンプライアンスと規制チェック**を含める必要があります。顧客のために機能するがデータプライバシー規則に違反する機能は、本当に「アウトプット完成」ではありません。

<!-- **How does this work in practice?** -->

**これは実際にはどのように機能しますか？**

<!-- - **Embed compliance** into the Definition of Output Done. This shifts compliance from a separate gate at the end to an integral element of the quality of every Increment in every Sprint. It becomes ingrained in the Product Developer's daily behavior.
- **Automate evidence collection.** Audit trails, test reports, and documentation should be generated as a byproduct of delivery, not as a scramble before release.
- **Use inspection and adaptation.** Regular reviews with compliance officers ensure evolving rules or deviations are addressed continuously, not retroactively.
- **Share the Definition of Output Done** at every Sprint Review. Build trust by being transparent about what "output done" means in terms of quality. _Do not demonstrate a not "output done" feature — that betrays trust._ -->

- **コンプライアンスを**アウトプット完成の定義に**組み込む**。これにより、コンプライアンスは終わりの別個のゲートから、毎スプリントのすべてのインクリメントの品質の不可欠な要素に移行します。それはプロダクト開発者の日々の行動に浸透します。
- **エビデンス収集を自動化する。** 監査証跡、テストレポート、ドキュメントは、リリース前の慌ただしい作業としてではなく、納品の副産物として生成されるべきです。
- **検査と適応を使用する。** コンプライアンス担当者との定期的なレビューにより、進化するルールや逸脱が遡及的にではなく継続的に対処されることを確保します。
- **アウトプット完成の定義を**毎回のスプリントレビューで**共有する**。「アウトプット完成」が品質の観点から何を意味するかについて透明であることで信頼を構築します。_「アウトプット完成」でない機能をデモンストレーションしないでください—それは信頼を裏切ります。_

<!-- Compliance is about **earned trust**. Customers trust that their data is safe, regulators trust that companies act responsibly, and leaders trust that teams deliver without exposing the organization to existential risks. Agility and compliance are not mutually exclusive; done right, they can help build a **competitive advantage**. -->

コンプライアンスは**獲得した信頼**についてです。顧客はデータが安全であることを信頼し、規制当局は企業が責任を持って行動することを信頼し、リーダーはチームが組織を存亡に関わるリスクにさらすことなく納品することを信頼します。アジリティとコンプライアンスは相互に排他的ではありません。正しく行えば、それらは**競争優位**を構築するのに役立ちます。

<!-- ### Ethics Guardrails – Working Within Boundaries -->

### 倫理的ガードレール – 境界内での作業 {#ethics-guardrails-working-within-boundaries}

<!-- Scrum requires teams to create products **within the ethical boundaries of their context**. This means teams must actively prevent harm while seeking outcomes and impacts. Guardrails include: -->

スクラムはチームに**文脈の倫理的境界内で**プロダクトを作成することを要求します。これはチームがアウトカムとインパクトを追求しながら積極的に害を防がなければならないことを意味します。ガードレールには以下が含まれます：

<!-- - **No dark patterns:** Avoid manipulative designs that trick users into actions.
- **Data minimization:** Collect only what is necessary, with explicit user consent.
- **Fairness and bias checks:** Ensure features and algorithms treat groups equitably.
- **Transparency:** Make terms, data use, and risks visible to users and stakeholders.
- **Accessibility as default:** Products must be usable by people of diverse abilities.
- **Safety reviews:** Include ethical and safety checks.
- **Responsible AI use:** Validate AI outputs for fairness, accuracy, and explainability; ensure humans remain accountable for critical decisions. -->

- **ダークパターンを使わない:** ユーザーを騙してアクションを取らせる操作的なデザインを避ける。
- **データの最小化:** 明示的なユーザーの同意を得て、必要なものだけを収集する。
- **公平性とバイアスのチェック:** 機能とアルゴリズムがグループを公平に扱うことを確保する。
- **透明性:** 利用規約、データ使用、リスクをユーザーとステークホルダーに可視化する。
- **デフォルトとしてのアクセシビリティ:** プロダクトは多様な能力を持つ人々が使用できなければならない。
- **安全性レビュー:** 倫理的および安全性チェックを含める。
- **責任あるAIの使用:** AI出力の公平性、正確性、説明可能性を検証する。重要な意思決定について人間が説明責任を持ち続けることを確保する。

<!-- Embedding these into the **Definition of Output Done** and **Definition of Outcome Done** ensures Scrum Teams deliver value **responsibly** and **sustainably**. -->

これらを**アウトプット完成の定義**と**アウトカム完成の定義**に組み込むことで、スクラムチームが**責任を持って**かつ**持続可能に**価値を提供することを確保します。

<!-- ## How to Put It into Action – Practical Guidance for Organizations -->

## 実践への移行 – 組織のための実践的ガイダンス {#how-to-put-it-into-action-practical-guidance-for-organizations}

<!-- ### For Teams – How to shift from output to outcome -->

### チーム向け – アウトプットからアウトカムへの移行方法 {#for-teams-how-to-shift-from-output-to-outcome}

<!-- - **Claim autonomy with intent:** Define clear Sprint Goals and agree as a Scrum Team how you'll reach them. Own the outcome and measure it, don't wait for step-by-step instructions.
- **Start with outcome & own the whole chain:** Map how your work links from task → feature → outcome → impact. Build telemetry into your product. Regularly check if you're still moving the needle.
- **Practice discovery and measurement:** Run small experiments (A/B tests, prototypes, user interviews). Track leading indicators (outputs), as well as lagging indicators (outcome/impact), and use results to adapt [^11].
- **Feasibility first:** Use spikes to derisk unknowns; review skills/dependencies each Sprint. -->

- **意図を持って自律性を主張する:** 明確なスプリントゴールを定義し、スクラムチームとしてそれをどのように達成するかを合意する。アウトカムを所有し測定する。ステップバイステップの指示を待たない。
- **アウトカムから始め、チェーン全体を所有する:** 作業がタスク → 機能 → アウトカム → インパクトにどのように結びつくかをマッピングする。プロダクトにテレメトリを組み込む。針が動いているかどうかを定期的に確認する。
- **発見と測定を実践する:** 小さな実験（A/Bテスト、プロトタイプ、ユーザーインタビュー）を実行する。先行指標（アウトプット）と遅行指標（アウトカム/インパクト）を追跡し、結果を使って適応する[^11]。
- **フィージビリティ優先:** スパイクを使って未知のものからリスクを取り除く。各スプリントでスキル/依存関係をレビューする。

<!-- ### For Leaders – How to enable outcome thinking -->

### リーダー向け – アウトカム思考を可能にする方法 {#for-leaders-how-to-enable-outcome-thinking}

<!-- - **Fund outcomes, not projects:** Allocate budgets to outcome‑related Product Goals, not fixed feature lists. Consider rolling budgets [^12] [^32].
- **Invest in stable Scrum Teams focusing on one Product:** A group of people working together is not a team; a team is an emergent property. Build great Scrum Teams and keep them together so they can build your products. Stable, empowered teams have far higher chances of outcome predictability. If there is unavoidable or deliberate dynamism in team membership, consider intentionally adopting Dynamic Reteaming [^33].
- **Use metrics intentionally:** Track metrics that reflect outcome and impact as well as your internal capabilities.
- **Balance deployment with emergence:** State the desired impact clearly, but let Scrum Teams experiment and discover how best to achieve it. Review and adjust strategy when new evidence emerges.
- **Watch viability:**
  Make sure that what was built has a positive impact on the organization. For commercial products, it may be useful to monitor LTV (Lifetime Value) or CAC (Customer Acquisition Cost). For tools built to support customers, monitor routine usage, and customer satisfaction. And for internal products, pay attention to measures of effectiveness and efficiency. All of these contribute to the impact, or viability, of solutions. -->

- **プロジェクトではなくアウトカムに資金を提供する:** 固定された機能リストではなく、アウトカム関連のプロダクトゴールに予算を割り当てる。ローリング予算を検討する[^12] [^32]。
- **1つのプロダクトに集中する安定したスクラムチームに投資する:** 一緒に働く人々のグループはチームではない。チームは創発的な特性である。素晴らしいスクラムチームを構築し、彼らがあなたのプロダクトを構築できるように一緒に保つ。安定した、エンパワーされたチームはアウトカムの予測可能性がはるかに高い。チームメンバーシップに避けられないまたは意図的なダイナミズムがある場合は、意図的にダイナミックリチーミングの採用を検討する[^33]。
- **意図的に指標を使用する:** アウトカムとインパクトを反映する指標と、内部能力を追跡する。
- **デプロイメントと創発のバランスを取る:** 望ましいインパクトを明確に述べるが、スクラムチームがそれを達成する最善の方法を実験し発見できるようにする。新しいエビデンスが出てきたら戦略をレビューし調整する。
- **実現可能性を監視する:**
  構築されたものが組織にポジティブなインパクトを与えていることを確認する。商用プロダクトの場合、LTV（顧客生涯価値）またはCAC（顧客獲得コスト）を監視することが有用かもしれない。顧客をサポートするために構築されたツールの場合、日常的な使用と顧客満足度を監視する。そして内部プロダクトの場合、有効性と効率性の指標に注意を払う。これらすべてがソリューションのインパクト、または実現可能性に貢献する。

<!-- ### For Stakeholders – How to experience the difference -->

### ステークホルダー向け – 違いを体験する方法 {#for-stakeholders-how-to-experience-the-difference}

<!-- - **Co‑create solutions:** If possible, attend or invite customers and users to Refinements, and provide or collect feedback through regular Sprint Reviews, user testing, and surveys.
- **Look for evidence of learning:** notice whether your pain points are being resolved and whether improvements are sustained.
- **Build trust over the long term:** Stick with products and teams that demonstrate consistency in learning, adapting, and delivering meaningful outcomes. -->

- **ソリューションを共同作成する:** 可能であれば、リファインメントに参加するか顧客やユーザーを招待し、定期的なスプリントレビュー、ユーザーテスト、調査を通じてフィードバックを提供または収集する。
- **学習のエビデンスを探す:** 自分の痛点が解決されているかどうか、改善が持続されているかどうかに気づく。
- **長期的に信頼を構築する:** 学習、適応、意味のあるアウトカムの提供において一貫性を示すプロダクトとチームに付き合い続ける。

<!-- ## Pitfalls to Avoid – And How to Steer Clear -->

## 避けるべき落とし穴 – そしてどのように回避するか {#pitfalls-to-avoid-and-how-to-steer-clear}

<!-- - **Vanity metrics:** Instead of tracking the number of downloads or story points, track retention, engagement, or customer value delivered.
- **Ritualistic Agile (often called Cargo-Cult):** Tie every Sprint Goal back to a Product‑ or Strategic Goal. Ask, _"How does this Sprint move us closer to impact?"_
- **Short‑termism:** Balance quick wins with investment in sustainable technology, user trust, and long‑term goals.
- **Losing sight of the why:** Start each Product Backlog Item refinement by asking, _"Which outcome does this serve?"_ and _"How will success be measured?"_
- **Risk blindness:** Break work into small bets, run time‑boxed experiments, and surface risks early. Use learning reviews to adapt rather than assuming the plan holds.
- **Ethical pitfalls:** Avoid dark patterns and addictive loops; measure **healthy** engagement (value-in-use) rather than just time‑on‑site. -->

- **バニティメトリクス:** ダウンロード数やストーリーポイントを追跡する代わりに、リテンション、エンゲージメント、または提供された顧客価値を追跡する。
- **儀式的アジャイル（しばしばカーゴカルトと呼ばれる）:** すべてのスプリントゴールをプロダクトゴールまたは戦略的ゴールに結びつける。_「このスプリントはインパクトにどのように近づけるか？」_と問う。
- **短期主義:** 迅速な勝利と持続可能な技術、ユーザーの信頼、長期的なゴールへの投資のバランスを取る。
- **なぜを見失う:** 各プロダクトバックログアイテムのリファインメントを_「これはどのアウトカムに貢献するか？」_と_「成功はどのように測定されるか？」_と問うことから始める。
- **リスク盲目:** 作業を小さな賭けに分割し、タイムボックス化された実験を実行し、リスクを早期に表面化させる。計画が維持されると仮定するのではなく、学習レビューを使って適応する。
- **倫理的な落とし穴:** ダークパターンと中毒性のあるループを避ける。単なるサイト滞在時間ではなく、**健全な**エンゲージメント（使用中の価値）を測定する。

<!-- ## Conclusion -->

## 結論 {#conclusion}

<!-- The Agile Manifesto was of its time - success was defined as delivering software output to clients. But the world has changed; the world of product development learned a lot in the last few decades. However, there is no single best practice; perspective matters. At a minimum, they must connect assumptions to inputs, inputs to activities, activities to outputs, outputs to outcomes, and outcomes to impacts. -->

アジャイルマニフェストはその時代のものでした—成功はクライアントにソフトウェアアウトプットを納品することとして定義されていました。しかし世界は変わりました。プロダクト開発の世界は過去数十年で多くを学びました。しかし、単一のベストプラクティスはありません。視点が重要です。少なくとも、仮定をインプットに、インプットを活動に、活動をアウトプットに、アウトプットをアウトカムに、アウトカムをインパクトに結びつけなければなりません。

<!-- **Impact** is what companies ultimately need for survival. **Outcomes** are about customer change, but impact is about whether the business thrives. It is the link between agility and strategy, between experiments and long-term direction. Companies that ignore impact risk become busy but irrelevant. Companies that embrace outcome-driven impact become resilient, adaptive, and sustainable. -->

**インパクト**は企業が最終的に生存のために必要とするものです。**アウトカム**は顧客の変化についてですが、インパクトはビジネスが繁栄するかどうかについてです。それはアジリティと戦略の間の、実験と長期的な方向性の間のリンクです。インパクトを無視する企業は忙しくなりますが、無関係になるリスクがあります。アウトカム駆動のインパクトを受け入れる企業はレジリエント、適応的、持続可能になります。

<!-- This requires a cultural shift — from **mercenaries to missionaries**, from **project thinking to product thinking**, from **circumstantial indicators to evidence‑informed management**. It also requires leaders to balance **strategy deployment** with **emergent strategy**; establish organizational transfer of learning and multi‑learning [^13] by setting ambitious goals, while allowing self‑managing Scrum Teams to discover the best path to achieve them. -->

これには文化的転換が必要です—**マーセナリーからミッショナリーへ**、**プロジェクト思考からプロダクト思考へ**、**状況的指標からエビデンスインフォームドマネジメントへ**。また、リーダーが**戦略展開**と**創発戦略**のバランスを取ることも必要です。野心的なゴールを設定することで組織的な学習の移転とマルチラーニング[^13]を確立し、同時に自己管理するスクラムチームがそれらを達成する最善の道を発見できるようにします。

<!-- **The path forward is clear:** -->

**前進への道は明確です：**

<!-- - Establish a **product approach**.
- Consider **EBM** or other approaches (e.g., adapted PDSA) to validate assumptions, measure outcomes and impacts, and make informed decisions.
- Apply **SGEP** to distinguish between "output done" and "outcome done"
- Consider adopting a continuous adaptive strategy.
- Build Scrum Teams that **own the entire product value stream**.
- Treat **impact** as the ultimate measure of success. -->

- **プロダクトアプローチ**を確立する。
- **EBM**またはその他のアプローチ（例：適応されたPDSA）を検討して、仮定を検証し、アウトカムとインパクトを測定し、情報に基づいた意思決定を行う。
- **SGEP**を適用して「アウトプット完成」と「アウトカム完成」を区別する。
- 継続的適応戦略の採用を検討する。
- **プロダクトバリューストリーム全体を所有する**スクラムチームを構築する。
- **インパクト**を成功の究極の尺度として扱う。

<!-- In short: **Stop celebrating cake recipes.** Start measuring how many people enjoyed the cake, came back for more, and kept the bakery thriving. -->

要するに：**ケーキのレシピを祝うのをやめてください。** ケーキを楽しんだ人、おかわりに来た人、ベーカリーを繁栄させ続けた人の数を測定し始めてください。

<!-- The most resilient companies keep the **why** and for **whom** of their strategy at the center. They manage risk not by pretending uncertainty can be eliminated, but by learning quickly and cheaply. They see variation as a benefit, and they understand competition not as a threat but as a forcing function to stay focused on outcomes and impacts that truly differentiate. When combined, these practices turn Scrum from a delivery engine into a **strategic advantage**. -->

最もレジリエントな企業は、戦略の**なぜ**と**誰のために**を中心に据えています。彼らは不確実性を排除できるふりをするのではなく、迅速かつ安価に学ぶことでリスクを管理します。彼らはばらつきを利点として見なし、競争を脅威としてではなく、真に差別化するアウトカムとインパクトに集中し続けるための強制関数として理解しています。これらのプラクティスを組み合わせると、スクラムは納品エンジンから**戦略的優位**に変わります。

<!-- Only then can Scrum be said to have fulfilled its promise - not just to build software, but to maximize customer value and create **lasting organizational impact**. -->

そうして初めてスクラムがその約束を果たしたと言えます—単にソフトウェアを構築するだけでなく、顧客価値を最大化し、**持続的な組織的インパクト**を創造すること。

<!-- ## References -->

## 参考文献 {#references}

[^1]: Beck, K. et al. (2001) _Manifesto for Agile Software Development_. Available at: [https://agilemanifesto.org](https://agilemanifesto.org) (Accessed: 20 September 2025).

[^2]: Beck, K. (2010) _To Agility, and Beyond_. Startup Lessons Learned Conference. Available at: [https://www.youtube.com/watch?v=d4qldY0g_dI](https://www.youtube.com/watch?v=d4qldY0g_dI) (Accessed: 20 September 2025).

[^3]: Gothelf, J. and Seiden, J. (2021) _Lean UX: Designing Great Products with Agile Teams_. 3rd ed. Sebastopol, CA: O'Reilly Media.

[^4]: Ries, E. (2011) _The Lean Startup: How Today's Entrepreneurs Use Continuous Innovation to Create Radically Successful Businesses_. New York: Crown.

[^5]: Scrum.org (2024) _Evidence-Based Management™ (EBM)_. Available at: [https://www.scrum.org/resources/evidence-based-management](https://www.scrum.org/resources/evidence-based-management) (Accessed: 20 September 2025).

[^7]: Duke, A. (2018) _Thinking in Bets: Making Smarter Decisions When You Don't Have All the Facts_. New York: Portfolio.

[^8]: Cagan, M. (2020) _Missionaries vs. Mercenaries_. Silicon Valley Product Group. Available at: [https://www.svpg.com/missionaries-vs-mercenaries/](https://www.svpg.com/missionaries-vs-mercenaries/) (Accessed: 20 September 2025).

[^9]: Cagan, M. (2018) _Inspired: How To Create Products Customers Love_. 2nd ed. Hoboken, NJ: Wiley.

[^10]: Schwaber, K. and Sutherland, J. (2020) _The Scrum Guide_. Available at: [https://scrumguides.org](https://scrumguides.org) (Accessed: 20 September 2025).

[^11]: Knapp, J., Zeratsky, J. and Kowitz, B. (2016) _Sprint: How to Solve Big Problems and Test New Ideas in Just Five Days_. New York: Simon & Schuster.

[^12]: Verma, R. et al. (2021) _10 Steps to Integrate Evidence-Based Management with Scrum in 21 Days or Less_. Scrum.org. Available at: [https://www.scrum.org/resources/10-steps-integrate-evidence-based-management-scrum-21-days-or-less](https://www.scrum.org/resources/10-steps-integrate-evidence-based-management-scrum-21-days-or-less) (Accessed: 20 September 2025).

[^13]: Takeuchi, H. and Nonaka, I. (2014) 'The New New Product Development Game', _Harvard Business Review_. Available at: [https://hbr.org/1986/01/the-new-new-product-development-game](https://hbr.org/1986/01/the-new-new-product-development-game) (Accessed: 20 September 2025).

[^14]: Sutherland, J., Jocham, R. and Coleman, J. (2025) _Scrum Guide Expansion Pack_. Available at: [https://scrumexpansion.org](https://scrumexpansion.org) (Accessed: 20 September 2025).

[^15]: Kaushik, A. (2009) _Web Analytics 2.0: The Art of Online Accountability and Science of Customer Centricity_. Indianapolis: Sybex.

[^16]: Cagan, M. (2023) _The Product Operating Model: An Introduction_. Silicon Valley Product Group. Available at: [https://www.svpg.com/the-product-operating-model-an-introduction/](https://www.svpg.com/the-product-operating-model-an-introduction/) (Accessed: 20 September 2025).

[^17]: Seiden, J. (2019) _Outcomes Over Output: Why Customer Behavior is the Key Metric for Business Success_. New York: Sense & Respond Press.

[^18]: McGreal, D. and Jocham, R. (2018) _The Professional Product Owner: Leveraging Scrum as a Competitive Advantage_. Boston, MA: Addison-Wesley Pearson.

[^19]: Cusumano, M.A. and Selby, R.W. (1995) _Microsoft Secrets: How the World's Most Powerful Software Company Creates Technology, Shapes Markets, and Manages People_. New York: Free Press.

[^20]: Amazon.com, Inc. (2010) _2009 Letter to Shareholders_. Available at: [https://www.sec.gov/Archives/edgar/data/1018724/000119312510082914/dex991.htm](https://www.sec.gov/Archives/edgar/data/1018724/000119312510082914/dex991.htm) (Accessed: 20 September 2025).

[^21]: Patton, J. (2014) _User story mapping: Discover the whole story, build the right product_. Sebastopol, CA: O'Reilly Media.

[^22]: Evolved Institute (2026) 'If the Agile Manifesto values were updated for 2026', _Evolved Institute Blog_, 15 January. Available at: [https://evolved.institute/blogs/news/if-the-agile-manifesto-values-were-updated-for-2026](https://evolved.institute/blogs/news/if-the-agile-manifesto-values-were-updated-for-2026) (Accessed: 21 January 2026).

[^24]: Riedesel, J. (2021) _Software Telemetry: Reliable Logging and Monitoring_. New York: Manning Publications.

[^25]: Beyer, B., Jones, C., Petoff, J. and Murphy, N.R. (2016) _Site Reliability Engineering: How Google Runs Production Systems_. Sebastopol, CA: O'Reilly Media.

[^26]: Deming, W.E. (1986) _Out of the crisis_. Cambridge, MA: Massachusetts Institute of Technology, Center for Advanced Engineering Study.

[^27]: Pfeffer, J. and Sutton, R.I. (2006) 'Evidence-based management', _Harvard Business Review_, 84(1), pp. 62-74.

[^28]: Sutherland, R. (2021) _Alchemy_. London: WH Allen. Available at: [https://www.penguin.co.uk/books/430379/alchemy-by-rory-sutherland/9780753556528](https://www.penguin.co.uk/books/430379/alchemy-by-rory-sutherland/9780753556528) (Accessed: 27 December 2025). To keep the insights from 'Alchemy' active and integrated into your strategic thinking, consider revisiting one rule of Alchemy each quarter. This cyclical practice can ensure that these innovative ideas remain a living part of your strategy, continually inspiring fresh approaches and guiding decision-making.

[^29]: MadFest London (2025) _Rory Sutherland on why being delightfully less wrong beats being boringly right_. Available at: [https://www.madfestlondon.com/insights/articles/rory-sutherland-on-why-being-delightfully-less-wrong-beats-being-boringly-right/](https://www.madfestlondon.com/insights/articles/rory-sutherland-on-why-being-delightfully-less-wrong-beats-being-boringly-right/) (Accessed: 27 December 2025).

[^30]: 42courses (2023) _Rory Sutherland's '11 Rules of Alchemy'_. Available at: [https://www.42courses.com/blog/home/rory-sutherlands-11-rules-of-alchemy](https://www.42courses.com/blog/home/rory-sutherlands-11-rules-of-alchemy) (Accessed: 27 December 2025).

[^31]: W.K. Kellogg Foundation (2004) _Logic Model Development Guide_. Battle Creek, MI: W.K. Kellogg Foundation. Available at: [https://wkkf.issuelab.org/resource/logic-model-development-guide.html](https://wkkf.issuelab.org/resource/logic-model-development-guide.html) (Accessed: 14 January 2026).

[^32]: Bogsnes, B. (2023) _Rethinking how we manage organizations in a post-industrial world, Beyond Budgeting_. Available at: [https://bbrt.org/wp-content/uploads/bb_principles.pdf](https://bbrt.org/wp-content/uploads/bb_principles.pdf) (Accessed: 5 April 2023).

[^33]: Helfand, H. (2019) _Dynamic Reteaming: The Art and Wisdom of Changing Teams_. 2nd edn. Walnut Creek, CA: O'Reilly Media.

[^34]: McChesney, C., Covey, S.R. and Huling, J. (2012) _The 4 Disciplines of Execution: Achieving Your Wildly Important Goals_. New York: Free Press.

---

## 本文書の用語 {#glossary}

本文書で使用される主な用語の解説です。Scrum Guide Expansion Packの他の文書で共通して使用される用語については、[用語集（スクラムガイド拡張パック 2026.1）]({{< ref "/scrum-guide-expanded/2026.1/index.ja.md#glossary" >}})を参照してください。

### プロダクト思考固有の用語

| 英語 | 日本語 | 説明 |
|------|--------|------|
| Product Thinking | プロダクト思考 | アウトプットの納品からアウトカムと長期的インパクトの所有へと移行する考え方 |
| Output | アウトプット | チームの活動から直接生み出される成果物（機能、インクリメント、標準など） |
| Outcome | アウトカム | 顧客の行動や体験における測定可能な変化 |
| Impact | インパクト | 収益成長、ROI改善、市場シェアなどの長期的な組織への影響 |
| Product Operating Model | プロダクト運用モデル | プロダクトの継続的な進化、学習、適応を期待する運用形態 |
| Project Operating Model | プロジェクト運用モデル | アウトプットで成功を測定する従来の運用形態 |
| Evidence-Based Management (EBM) | エビデンスベースドマネジメント | 価値提供を管理・改善するためのフレームワーク |
| Current Value (CV) | 現在価値 | 顧客・ユーザー・組織が今日受け取っている価値の量 |
| Unrealized Value (UV) | 未実現価値 | まだ残っている潜在的価値の量 |
| Ability to Innovate (A2I) | イノベーション能力 | 組織が改善・適応する能力 |
| Time to Market (T2M) | 市場投入時間 | 新しい価値を提供できる速度 |
| Definition of Output Done | アウトプット完成の定義 | インクリメントが品質基準を満たすことを保証する定義 |
| Definition of Outcome Done | アウトカム完成の定義 | リリースされたプロダクトが意図した顧客変化とビジネス結果を達成したかを問う定義 |
| Leading Indicators | 先行指標 | 進む方向についてのガイダンスを提供する早期シグナル |
| Lagging Indicators | 遅行指標 | 過去の行動の実際のインパクトを示す結果の測定 |
| Missionary Team | ミッショナリーチーム | 問題解決に深く関心を持ち、完全なバリューストリームを所有するチーム |
| Mercenary Team | マーセナリーチーム | 言われたことを納品するが、アウトカムを所有しないチーム |
| HiPPO Decision | HiPPO決定 | 最も給与の高い人の意見（Highest Paid Person's Opinion）に従う意思決定 |
| Vanity Metrics | バニティメトリクス | 見栄えは良いが実際の価値を反映しない指標 |
| Telemetry | テレメトリ | 使用データの自動収集 |
| PDSA Cycle | PDSAサイクル | Plan-Do-Study-Actの学習ループ |
| Psycho-logic | サイコロジック | 論理に反するように見えるが効果的な心理学的アプローチ |
| Failure Demand | 失敗需要 | 価値需要の反対で、失敗や問題から発生する需要 |
| Dynamic Reteaming | ダイナミックリチーミング | チームメンバーシップの意図的なダイナミズムを採用するアプローチ |

