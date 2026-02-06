---
# title: AI and Scrum (Expansion of the SGEP)
title: AIとスクラム（SGEP拡張版）
# subtitle: An Evidence-Informed Integration Guide
subtitle: エビデンスに基づく統合ガイド
# description: AI can accelerate delivery, but it can also scale waste if you build the wrong things faster. This guide shows how Scrum's transparency, inspection, and adaptation keeps humans accountable, protects quality, and turns AI-accelerated output into measurable outcomes, with practical guidance for Product Owners, Product Developers, Scrum Masters, and leaders.
description: AIはデリバリーを加速できるが、間違ったものをより速く構築すれば無駄も拡大する。このガイドでは、スクラムの透明性、検査、適応が人間の説明責任を維持し、品質を保護し、AI加速されたアウトプットを測定可能なアウトカムに変える方法を、プロダクトオーナー、プロダクト開発者、スクラムマスター、リーダー向けの実践的なガイダンスとともに示す。
# keywords:
# - AI-accelerated delivery
# - Outcome-driven product development
# - Empirical process control
# - Human accountability
keywords:
  - AI加速デリバリー
  - アウトカム駆動プロダクト開発
  - 経験的プロセス制御
  - 人間の説明責任
author:
  - Ralph Jocham
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
sitemap:
  priority: 0.8
aliases:
  - /ja/ai-and-scrum/2026.1/
---

<!-- ***Collected Resources for *Scrum Guide Expansion Pack**** -->

**_スクラムガイド拡張パック 収録資料集_**

<!-- *This document is a collection of independent works. Each section retains its original license or copyright status, as indicated. Please refer to each section for specific usage rights and requirements.* -->

_この文書は独立した著作物のコレクションである。各セクションは示されているとおり、元のライセンスまたは著作権の状態を保持している。具体的な使用権と要件については、各セクションを参照してほしい。_

---

<!-- ## Introduction -->

## はじめに {#introduction}

<!-- In the current era of rapid advances in artificial intelligence (AI), integrating AI into Scrum-based digital product development is not just an opportunity but an essential for maintaining relevance and competitiveness. This practical guide is intended for Scrum Teams (including Product Owners, Product Developers, Scrum Masters), and organizational leaders who seek to leverage AI responsibly while upholding Scrum's core principles of empiricism, transparency, and human accountability. It synthesizes the latest research to identify what distinguishes successful AI adopters from those struggling, and provides evidence-based guidance for responsible AI adoption within the Scrum framework. -->

人工知能（AI）が急速に進歩する現代において、AIをスクラムベースのデジタルプロダクト開発に統合することは、単なる機会ではなく、関連性と競争力を維持するために不可欠である。この実践的なガイドは、スクラムの経験主義、透明性、人間の説明責任という中核原則を堅持しながら、AIを責任を持って活用しようとするスクラムチーム（プロダクトオーナー、プロダクト開発者、スクラムマスターを含む）と組織リーダーを対象としている。成功するAI導入者と苦戦している者を区別するものを特定するために最新の研究を統合し、スクラムフレームワーク内での責任あるAI導入のためのエビデンスに基づくガイダンスを提供する。

<!-- The urgency of AI integration cannot be overstated. AI systems' ability to autonomously complete complex, extended tasks has been increasing at an exponential rate – roughly doubling every six to seven months [^1]. The competitive landscape has effectively shifted from linear to exponential growth in capabilities [^2]. -->

AI統合の緊急性はいくら強調してもしすぎることはない。AIシステムが複雑で長期的なタスクを自律的に完了する能力は、指数関数的な速度で増加している - およそ6〜7ヶ月ごとに倍増している [^1]。競争環境は事実上、能力の線形成長から指数関数的成長へとシフトした [^2]。

<!-- Industry analyses warn that organizations that delay AI adoption risk strategic obsolescence, as the gap between "AI-native" and "AI-laggard" firms is widening into a structural divide that could lead to mass disruption, consolidation, or even the extinction of slow adopters [^3] [^4]. In short, AI integration is no longer merely an evolution of how we work – it is a race against irrelevance. -->

業界分析は、AI導入を遅らせる組織は戦略的陳腐化のリスクがあると警告している。「AIネイティブ」企業と「AI後進」企業の間のギャップは、大規模な破壊、統合、または遅れた導入者の絶滅につながる可能性のある構造的な分断へと拡大している [^3] [^4]。要するに、AI統合はもはや単なる働き方の進化ではなく、無関係化との競争である。

<!-- This guide argues that Scrum's empirical process control and emphasis on human judgment provide a strong foundation for integrating AI responsibly at scale—*provided that organizations also evolve their assurance systems (quality, security, privacy, and auditability), decision rights, and feedback loops to keep pace with AI-driven speed.* -->

このガイドでは、スクラムの経験的プロセス制御と人間の判断の重視が、AIを責任を持って大規模に統合するための強固な基盤を提供すると主張する - *ただし、組織が品質保証システム（品質、セキュリティ、プライバシー、監査可能性）、意思決定権、フィードバックループをAI駆動の速度に追いつくよう進化させることを条件とする。*

<!-- Using the lens of the *Scrum Guide Expansion Pack* [^5] and current AI trends, we illustrate why Scrum is a resilient basis for implementing AI at scale. The SGEP view is that Scrum is mutable (the 2020 Scrum Guide considers it immutable); few noticed this change in June 2025. The SGEP explains the value of each part of Scrum so adopters can adapt with better knowledge. So, here "Scrum" also means adaptations to Scrum that are coherent with the SGEP. -->

*スクラムガイド拡張パック* [^5] と現在のAIトレンドのレンズを通して、スクラムがAIを大規模に実装するための回復力のある基盤である理由を説明する。SGEPの見解では、スクラムは可変である（2020年のスクラムガイドでは不変とみなされている）。2025年6月のこの変化に気づいた人はほとんどいなかった。SGEPはスクラムの各部分の価値を説明し、導入者がより良い知識で適応できるようにしている。したがって、ここでの「スクラム」は、SGEPと一貫性のあるスクラムへの適応も意味する。

<!-- The remainder of this guide is structured as follows. **Part 1 (What We Know)** reviews current evidence on AI's impact on software development. **Part 2 (What This Means)** analyzes the strategic implications of these findings for organizations and teams. **Part 3 (What Good Looks Like)** describes characteristics of successful AI integration observed in practice. Finally, **Part 4 (What To Do)** provides practical implementation guidance, tailored to Scrum roles and organizational readiness. -->

このガイドの残りの部分は以下のように構成されている。**パート1（私たちが知っていること）**は、ソフトウェア開発に対するAIの影響に関する現在のエビデンスをレビューする。**パート2（これが意味すること）**は、組織とチームに対するこれらの発見の戦略的意味を分析する。**パート3（良い状態とはどのようなものか）**は、実践で観察された成功するAI統合の特徴を説明する。最後に、**パート4（何をすべきか）**は、スクラムの役割と組織の準備状況に合わせた実践的な実装ガイダンスを提供する。

<!-- ## Part 1: What We Know – The Evidence -->

## パート1：私たちが知っていること - エビデンス {#part-1-what-we-know-the-evidence}

<!-- ### AI's Accelerating Capability Curve -->

### AIの加速する能力曲線 {#ais-accelerating-capability-curve}

<!-- The pace of AI improvement has been exponential. In 2023, early general AI models (like GPT-4) could roughly match a junior developer's ability on coding tasks, but often produced as many bugs as they fixed. Extensive human oversight was needed to ensure quality. By 2024, next-generation models (GPT-4.5, Claude 3.5, etc.) were performing more closely to a competent senior developer and generating much cleaner code. These improved capabilities shifted the bottleneck from coding to deciding what to build – teams found the AI could create features faster than the organization could validate their desirability. Strong Product Owners and Product Developers became critical to effectively directing AI efforts. -->

AIの改善ペースは指数関数的であった。2023年、初期の汎用AIモデル（GPT-4など）はコーディングタスクでジュニア開発者の能力にほぼ匹敵できたが、修正したのと同じくらい多くのバグを生成することが多かった。品質を確保するには広範な人間の監視が必要だった。2024年までに、次世代モデル（GPT-4.5、Claude 3.5など）は有能なシニア開発者により近いパフォーマンスを発揮し、はるかにクリーンなコードを生成するようになった。これらの改善された能力により、ボトルネックはコーディングから何を構築するかの決定へとシフトした - チームは、AIが組織がその望ましさを検証できるよりも速く機能を作成できることを発見した。強力なプロダクトオーナーとプロダクト開発者が、AI の取り組みを効果的に方向付けるために重要になった。

<!-- By 2025, frontier models like GPT-5 and Claude 4 achieved expert-level performance. In controlled settings, coding errors became rare; instead, the risk was building the wrong product. The key question became "should we build it (and why)?", rather than "can AI build it?". Product management overtook engineering as the limiting factor in value delivery. Notably, although 78% of companies were using AI by 2025, about 80% reported no significant business impact [^3] [^4] – a "generative AI paradox" attributed to teams producing features without sufficient product guidance or validation. -->

2025年までに、GPT-5やClaude 4などのフロンティアモデルは専門家レベルのパフォーマンスを達成した。管理された環境では、コーディングエラーは稀になった。代わりに、リスクは間違ったプロダクトを構築することになった。重要な問いは「AIが構築できるか？」ではなく「構築すべきか（なぜ）？」になった。プロダクトマネジメントが価値提供の制限要因としてエンジニアリングを追い越した。注目すべきことに、2025年までに企業の78%がAIを使用していたが、約80%が重大なビジネスインパクトを報告していない [^3] [^4] - これは十分なプロダクトガイダンスや検証なしに機能を生産するチームに起因する「生成AIパラドックス」である。

<!-- By 2026 and beyond, AI systems will begin to exceed human expert capabilities in narrow tasks (some models approaching a genius-level). A few leading organizations have redesigned their workflows entirely around AI – in some cases, letting AI agents handle routine tasks – and have started to see exponential performance gains. Meanwhile, the majority still struggle to translate AI into bottom-line value [^3]. By 2027, AI models (e.g., a future GPT-6) may surpass an IQ equivalent of 200, entering superhuman territory. At that point, the challenge will be human comprehension, built-in quality, and control: Product Owners will need to act as cognitive orchestrators, setting intent and constraints for super-intelligent AI and ensuring outcomes align with organizational goals and values [^17] [^18]. In effect, as AI's technical capacity surges, the human ability to steer that capacity toward valuable ends becomes the defining constraint. -->

2026年以降、AIシステムは狭いタスクで人間の専門家の能力を超え始める（一部のモデルは天才レベルに近づいている）。いくつかの先進的な組織はワークフロー全体をAI中心に再設計し - 場合によってはAIエージェントに日常的なタスクを処理させ - 指数関数的なパフォーマンス向上を見始めている。一方、大多数は依然としてAIを収益価値に変換するのに苦労している [^3]。2027年までに、AIモデル（例えば将来のGPT-6）はIQ200相当を超え、超人的な領域に入る可能性がある。その時点で、課題は人間の理解、組み込み品質、制御になる：プロダクトオーナーは認知オーケストレーターとして行動し、超知能AIの意図と制約を設定し、アウトカムが組織の目標と価値観に整合することを確保する必要がある [^17] [^18]。事実上、AIの技術的能力が急増するにつれて、その能力を価値ある目的に向けて操縦する人間の能力が決定的な制約となる。

<!-- ### Adoption Reality: Rapid Uptake with Trust Gaps -->

### 導入の現実：信頼ギャップを伴う急速な普及 {#adoption-reality-rapid-uptake-with-trust-gaps}

<!-- AI development tools have seen widespread, rapid adoption among software professionals. By late 2025, an estimated 84% of developers report using AI coding tools in some capacity, with over half using them daily [^6]. Code generation assistants like GitHub Copilot are especially popular, with 63% of professional developers using them [^6]. However, this enthusiastic uptake is tempered by significant issues of trust and reliability. Product Developer confidence in the accuracy of AI outputs has declined as usage increased—surveys show trust in AI-generated code dropped from 69% in 2024 to only 54% in 2025 [^6]. -->

AI開発ツールは、ソフトウェア専門家の間で広範かつ急速に採用されている。2025年後半までに、推定84%の開発者が何らかの形でAIコーディングツールを使用していると報告しており、半数以上が毎日使用している [^6]。GitHub Copilotのようなコード生成アシスタントは特に人気があり、プロの開発者の63%が使用している [^6]。しかし、この熱心な採用は、信頼性と信頼性の重大な問題によって和らげられている。AI出力の精度に対するプロダクト開発者の信頼は、使用が増加するにつれて低下した - 調査によると、AI生成コードへの信頼は2024年の69%から2025年にはわずか54%に低下した [^6]。

<!-- The most common frustration is getting solutions that are "almost right, but not quite"—the AI's output appears plausible yet contains subtle errors that create additional work to detect and correct. These findings echo broader concerns about large language models producing fluent but potentially misleading outputs [^7]. In effect, many teams adopt the tools quickly, but then spend substantial time double-checking and correcting AI output. Dave Farley suggests manually creating Specification by Example test harnesses, as the AI cannot be trusted to "mark its own homework"; the specificity of SbE provides the concrete, testable expectations that AI needs to translate qualitative prompts into verifiable behavior. -->

最も一般的なフラストレーションは、「ほぼ正しいが、完全ではない」ソリューションを得ることである - AIの出力はもっともらしく見えるが、検出と修正に追加の作業を生む微妙なエラーを含んでいる。これらの発見は、大規模言語モデルが流暢だが潜在的に誤解を招く出力を生成することに関するより広い懸念を反映している [^7]。事実上、多くのチームはツールを素早く採用するが、その後AI出力のダブルチェックと修正にかなりの時間を費やす。Dave Farleyは、AIは「自分の宿題を採点する」ことを信頼できないため、実例による仕様（Specification by Example）のテストハーネスを手動で作成することを提案している。SbEの具体性は、AIが定性的なプロンプトを検証可能な振る舞いに変換するために必要な具体的でテスト可能な期待を提供する。

<!-- Compounding this is a productivity paradox. On the surface, self-reported productivity is up: 78% of developers using AI report that it makes them more productive [^8]. At the same time, 76% of these developers report they do not fully trust AI-generated code [^8]. In practice, experienced engineers often find that for complex tasks, the overhead of vetting AI-generated output can reduce or even negate productivity gains. One study found that senior developers experienced about a 19% decrease in performance on complicated coding tasks when using an AI assistant, due to the time spent reviewing and testing the AI's work [^8]. In other words, speed gains from AI drafting can be offset by verification costs. Without process changes, AI's promised efficiency risks turning into a situation where developers do two jobs—building software and policing the AI—which is not sustainable. -->

これに加えて生産性パラドックスがある。表面上、自己報告の生産性は上昇している：AIを使用する開発者の78%が、それによってより生産的になったと報告している [^8]。同時に、これらの開発者の76%がAI生成コードを完全には信頼していないと報告している [^8]。実際には、経験豊富なエンジニアは、複雑なタスクについて、AI生成出力の検証のオーバーヘッドが生産性向上を減少させるか、さらには相殺する可能性があることをしばしば発見する。ある研究では、シニア開発者がAIアシスタントを使用した場合、AIの作業のレビューとテストに費やす時間のために、複雑なコーディングタスクでパフォーマンスが約19%低下したことが判明した [^8]。言い換えれば、AIドラフトによるスピード向上は検証コストによって相殺される可能性がある。プロセスの変更なしには、AIの約束された効率性は、開発者がソフトウェア構築とAIの監視という2つの仕事をする状況に変わるリスクがある - これは持続可能ではない。

<!-- ### Code Quality and Failure Patterns -->

### コード品質と失敗パターン {#code-quality-and-failure-patterns}

<!-- Despite rapid tool adoption at the developer level, scaling AI initiatives to production remains uneven; Gartner (2022) reports that on average, 54% of AI projects make it from pilot to production, implying that a substantial share do not reach production at all [^11]. -->

開発者レベルでのツールの急速な採用にもかかわらず、AIイニシアチブを本番環境にスケールすることは依然として不均一である。Gartner（2022）は、平均してAIプロジェクトの54%がパイロットから本番に移行すると報告しており、かなりの割合が本番に到達しないことを示唆している [^11]。

<!-- Early evidence from real-world projects suggests that introducing AI into development can degrade code quality if not carefully managed. Analyses of large codebases have found troubling patterns as AI coding assistance became more common. For example, code duplication in some AI-assisted projects increased significantly (from \~8% to \~12% of lines changed), and refactoring activity – developers improving existing code – dropped sharply as teams pumped out new code instead of refining it [^9] [^10]. -->

実世界のプロジェクトからの初期のエビデンスは、慎重に管理されない場合、AIを開発に導入するとコード品質が低下する可能性があることを示唆している。AIコーディング支援がより一般的になるにつれて、大規模なコードベースの分析で厄介なパターンが発見された。例えば、一部のAI支援プロジェクトでは、コードの重複が大幅に増加し（変更された行の約8%から約12%へ）、リファクタリング活動 - 開発者が既存のコードを改善すること - は、チームがコードを洗練する代わりに新しいコードを大量生産するにつれて急激に減少した [^9] [^10]。

<!-- In 2024, observers noted that, for the first time, copy-pasted or AI-generated code additions exceeded refactored code edits [^10]. This indicates that without deliberate safeguards, AI can tempt teams to prioritize speed over craftsmanship or engineering. The result is accumulating technical debt or a mess – a growing burden of messy, fragile code that may work initially but becomes costly to maintain. In short, AI lets you go faster, but if that speed comes without improved practices, you simply accelerate the rate at which your codebase becomes complex and error-prone. -->

2024年、観察者たちは初めて、コピーペーストまたはAI生成のコード追加がリファクタリングされたコード編集を上回ったことに気づいた [^10]。これは、意図的なセーフガードなしでは、AIがチームにクラフトマンシップやエンジニアリングよりもスピードを優先させる誘惑を与える可能性があることを示している。結果は技術的負債または混乱の蓄積である - 最初は機能するかもしれないが、維持するのにコストがかかる、乱雑で脆弱なコードの増大する負担。要するに、AIはより速く進むことを可能にするが、そのスピードが改善されたプラクティスなしに来る場合、コードベースが複雑でエラーが発生しやすくなる速度を単に加速するだけである。

<!-- Common causes include treating AI as a superficial add-on rather than redesigning workflows; a lack of supporting processes (such as robust testing and validation of AI outputs); organizational resistance to the changes in roles and habits AI necessitates; and a mismatch between fast AI-driven development and slower legacy release or feedback processes. The net effect is a two-speed IT reality: many organizations accelerate development with AI only to hit bottlenecks in quality assurance, user testing, or stakeholder review. -->

一般的な原因には、ワークフローを再設計するのではなくAIを表面的なアドオンとして扱うこと、支援プロセスの欠如（AI出力の堅牢なテストと検証など）、AIが必要とする役割と習慣の変化に対する組織的な抵抗、高速なAI駆動開発と遅いレガシーリリースまたはフィードバックプロセスとのミスマッチが含まれる。正味の効果は二速度のIT現実である：多くの組織がAIで開発を加速するが、品質保証、ユーザーテスト、またはステークホルダーレビューでボトルネックにぶつかるだけである。

<!-- Only a small elite has managed to align their entire system (people, processes, and technology) to capitalize on AI fully. These high performers build closed-loop feedback into their AI workflows (catching errors early with automated checks), give AI tools rich context (e.g., company-specific training data) to improve relevance, and redesign roles and norms to make AI a core part of the process rather than a novelty. Such organizations report substantial productivity gains while maintaining quality, whereas the rest see at best modest gains offset by new challenges [^8]. -->

少数のエリートだけがシステム全体（人、プロセス、テクノロジー）を調整してAIを完全に活用することに成功した。これらのハイパフォーマーは、AIワークフローにクローズドループフィードバックを構築し（自動チェックで早期にエラーをキャッチ）、AIツールに豊富なコンテキスト（例：企業固有のトレーニングデータ）を提供して関連性を向上させ、AIを目新しいものではなくプロセスの中核部分にするために役割と規範を再設計する。このような組織は品質を維持しながら大幅な生産性向上を報告しているが、残りは新しい課題によって相殺される控えめな向上を見るのがせいぜいである [^8]。

<!-- ## Part 2: What This Means – Strategic Implications -->

## パート2：これが意味すること - 戦略的意味 {#part-2-what-this-means-strategic-implications}

<!-- **AI's impact on Scrum Teams creates a fundamental paradox:** it accelerates output but does not automatically guarantee outcomes. To convert increased development speed into real customer value, organizations must evolve not only their technical practices but also their management and product strategies—especially how decisions are made. In an AI-accelerated environment, centralized approval chains and slow, hierarchical prioritization become bottlenecks; value requires distributed decision making within clear strategic guardrails, so teams can quickly choose, test, and adapt based on evidence rather than waiting for permission. -->

**スクラムチームに対するAIの影響は根本的なパラドックスを生み出す：** アウトプットを加速するが、自動的にアウトカムを保証するわけではない。増加した開発スピードを実際の顧客価値に変換するために、組織は技術的なプラクティスだけでなく、マネジメントとプロダクト戦略 - 特に意思決定の方法 - も進化させなければならない。AI加速環境では、中央集権的な承認チェーンと遅い階層的な優先順位付けがボトルネックになる。価値は、明確な戦略的ガードレール内での分散型意思決定を必要とし、チームが許可を待つのではなく、エビデンスに基づいて迅速に選択、テスト、適応できるようにする。

<!-- **Speed without Direction:** The chief risk is that AI enables the wrong things to be built faster. Without a strong Product Goal and fast feedback loops, teams can become high-throughput "feature factories," producing lots of features that do not solve real problems [^12]. The presence of AI magnifies strengths and weaknesses. If your Scrum practice is sound (empirically guided, rhythmic in a direction of travel, professional, disciplined, psychologically safe, and value-focused), AI can amplify its effectiveness; if your process lacks clear direction or quality discipline, AI will amplify the dysfunction. As one observer noted, if you have a broken compass, running faster just gets you lost more quickly. -->

**方向性のないスピード：** 主なリスクは、AIが間違ったものをより速く構築することを可能にすることである。強力なプロダクトゴールと迅速なフィードバックループなしでは、チームは高スループットの「フィーチャーファクトリー」になり、実際の問題を解決しない多くの機能を生産する可能性がある [^12]。AIの存在は強みと弱みを拡大する。スクラムプラクティスが健全（経験的にガイドされ、進行方向にリズミカルで、プロフェッショナルで、規律があり、心理的に安全で、価値に焦点を当てている）であれば、AIはその効果を増幅できる。プロセスに明確な方向性や品質規律が欠けている場合、AIは機能不全を増幅する。ある観察者が指摘したように、壊れたコンパスを持っている場合、より速く走ることはより早く迷子になるだけである。

<!-- Many organizations have historically optimized for ease of management—predictability, reporting, centralized control, and approval structures—rather than ease of delivery. AI acts as a magnifying glass on this imbalance. When work is optimized for managerial convenience rather than fast learning and delivery, AI does not fix the system; it accelerates local output while amplifying systemic dysfunction. In such environments, AI enables teams to build the wrong things faster, increasing waste rather than value. -->

多くの組織は歴史的に、デリバリーの容易さではなく、マネジメントの容易さ - 予測可能性、レポーティング、中央集権的な制御、承認構造 - のために最適化してきた。AIはこのアンバランスに対する拡大鏡として機能する。作業が迅速な学習とデリバリーではなく管理上の便宜のために最適化されている場合、AIはシステムを修正しない。システム的な機能不全を増幅しながらローカルなアウトプットを加速する。このような環境では、AIはチームが間違ったものをより速く構築することを可能にし、価値ではなく無駄を増加させる。

<!-- **Exponential Change, Short Window:** As AI capabilities improve at an exponential rate and are rapidly adopted across industries, organizations face a narrow window to adapt. Practically, experts suggest that companies have about 12–24 months to achieve meaningful AI integration before falling too far behind [^3]. This is not hyperbole; it reflects exponential curves: a few months' delay now could translate into years behind a competitor that is compounding its learning and capabilities. Market trends already show early adopters pulling ahead via network effects and data advantages that latecomers will struggle to catch up to [^4]. The implication is clear – a sense of urgency must permeate the delivery of outcomes in a direction. AI adoption is no longer a "wait and see" proposition; it's adapt soon or risk irrelevance. -->

**指数関数的変化、短い時間枠：** AI能力が指数関数的な速度で向上し、業界全体で急速に採用されるにつれて、組織は適応するための狭い時間枠に直面している。実際的には、専門家は、企業が遅れすぎる前に意味のあるAI統合を達成するには約12〜24ヶ月あると示唆している [^3]。これは誇張ではない。指数曲線を反映している：今の数ヶ月の遅れは、学習と能力を複利で増やしている競合他社の数年後ろになる可能性がある。市場のトレンドはすでに、後発者が追いつくのに苦労するネットワーク効果とデータの優位性を通じて、早期採用者が先行していることを示している [^4]。含意は明確である - 緊急感が方向性のあるアウトカムのデリバリーに浸透しなければならない。AI導入はもはや「様子見」の提案ではない。すぐに適応するか、無関係になるリスクを負うかである。

<!-- ### **Key Tensions to Manage** -->

### 管理すべき主要な緊張関係 {#key-tensions-to-manage}

<!-- **In pursuing AI integration, organizations must deliberately balance several inherent tensions:** -->

**AI統合を追求する際、組織はいくつかの固有の緊張関係を意図的にバランスさせなければならない：**

<!-- - **Structure vs. Agency:** AI accelerates speed and thereby the need for cross-functional collaboration, and the feasibility of distributed decision-making. Traditional hierarchical organization structures (organization charts, functional silos, centralized approvals) might still matter for legal accountability and people management—but they often become poor representations of how value is created and how decisions flow [^19]. If the organization relies solely on the hierarchy to coordinate work, AI will simply accelerate local output while amplifying enterprise bottlenecks (handoffs, queues, approvals). Managing this tension means keeping the org chart as the accountability skeleton while operating day to day through value streams, clear decision rights, and empowered teams. Leaders must define strategic intent and guardrails (risk, compliance, quality, context-specific ethics), then deliberately push decision authority to the lowest responsible level so teams can act, learn, and adapt quickly based on evidence. -->

- **構造 vs. 主体性：** AIはスピードを加速し、それによって機能横断的なコラボレーションの必要性と分散型意思決定の実現可能性を高める。伝統的な階層的組織構造（組織図、機能別サイロ、中央集権的承認）は、法的説明責任と人材管理のためにまだ重要かもしれないが、価値がどのように創造され、意思決定がどのように流れるかの貧弱な表現になることが多い [^19]。組織が作業を調整するために階層にのみ依存している場合、AIはエンタープライズのボトルネック（引き継ぎ、キュー、承認）を増幅しながらローカルなアウトプットを単に加速するだけである。この緊張を管理することは、組織図を説明責任の骨格として維持しながら、バリューストリーム、明確な意思決定権、エンパワーメントされたチームを通じて日々運営することを意味する。リーダーは戦略的意図とガードレール（リスク、コンプライアンス、品質、コンテキスト固有の倫理）を定義し、チームがエビデンスに基づいて迅速に行動、学習、適応できるように、意思決定権限を最も低い責任レベルに意図的に押し下げなければならない。

<!-- - **Speed vs. Quality**: AI can dramatically accelerate development, but moving faster can compromise quality unless active measures are taken. Without guardrails, teams accumulate technical debt faster than they can pay it down. Declining code quality has already been observed in some AI-adopting teams [^10]. Managing this tension means investing in automated testing, refactoring, and a stricter Definition of Output Done to keep quality constant even as velocity increases. Leadership must send the message that quality is not negotiable – speed is beneficial only if you can maintain quality. -->

- **スピード vs. 品質：** AIは開発を劇的に加速できるが、積極的な対策を講じなければ、より速く動くことは品質を損なう可能性がある。ガードレールなしでは、チームは返済できるよりも速く技術的負債を蓄積する。コード品質の低下は、一部のAI導入チームですでに観察されている [^10]。この緊張を管理することは、速度が増加しても品質を一定に保つために、自動テスト、リファクタリング、より厳格なアウトプット完成の定義に投資することを意味する。リーダーシップは、品質は交渉の余地がないというメッセージを送らなければならない - スピードは品質を維持できる場合にのみ有益である。

<!-- - **Automation vs. Accountability**: As AI automates more tasks, human team members may feel less ownership of outcomes. The attitude "the AI suggested it, so we implemented it" can lead to diffused responsibility. This is dangerous because it undermines learning and accountability. To address this, teams should make it clear that AI is a tool and that humans remain accountable for decisions and results. Research on human–automation interaction warns of automation bias and complacency – people may over-trust automated systems and become passive in oversight [^13] [^14]. Scrum Teams must consciously keep a human-in-the-loop attitude: AI may recommend, but humans decide. -->

- **自動化 vs. 説明責任：** AIがより多くのタスクを自動化するにつれて、人間のチームメンバーはアウトカムに対するオーナーシップを感じにくくなる可能性がある。「AIが提案したから実装した」という態度は、責任の拡散につながる可能性がある。これは学習と説明責任を損なうため危険である。これに対処するために、チームはAIがツールであり、人間が意思決定と結果に対して説明責任を負い続けることを明確にすべきである。人間と自動化の相互作用に関する研究は、自動化バイアスと自己満足について警告している - 人々は自動化されたシステムを過度に信頼し、監視において受動的になる可能性がある [^13] [^14]。スクラムチームは意識的にヒューマン・イン・ザ・ループの態度を維持しなければならない：AIは推奨するかもしれないが、人間が決定する。

<!-- - **Outputs vs. Outcomes**: AI makes it easy to measure outputs (e.g., lines of code generated, features delivered), but organizations must resist the urge to be activity- or output-driven and remain outcome-driven. The objective measure of success is whether those AI-accelerated outputs provide valuable outcomes for users and business impact. This means doubling down on practices such as defining clear Product Goals, defining feature success metrics, and using hypothesis-driven development. It may be tempting to celebrate how many Product Backlog items an AI completes, but Scrum teams should instead ask, "What measurable benefit did this deliver?" to ensure they are not just doing more busy work faster. -->

- **アウトプット vs. アウトカム：** AIはアウトプット（例：生成されたコード行数、デリバリーされた機能）を測定することを容易にするが、組織は活動やアウトプット駆動になる衝動に抵抗し、アウトカム駆動であり続けなければならない。成功の客観的な尺度は、それらのAI加速されたアウトプットがユーザーに価値あるアウトカムとビジネスインパクトを提供するかどうかである。これは、明確なプロダクトゴールの定義、機能の成功指標の定義、仮説駆動開発の使用などのプラクティスを倍増させることを意味する。AIが完了したプロダクトバックログアイテムの数を祝いたくなるかもしれないが、スクラムチームは代わりに「これは何の測定可能な利益をデリバリーしたか？」と問い、単により多くの忙しい仕事をより速くやっているだけではないことを確認すべきである。

<!-- - **Tool Adoption vs. System Transformation**: Simply rolling out AI tools will yield limited benefit if the surrounding system (process, roles, culture) has not evolved. Many failed pilots stem from trying to "plug in" AI to an unchanged organization. Real gains come when workflows are redesigned around AI's strengths. This could mean changing how work is sliced (perhaps into smaller increments that AI can tackle), adjusting event cadences (for example, more frequent reviews to accelerate cycles), or evolving accountabilities (for example, curious, rounded, and flexible Product Developers spending more time on oversight and design). In short, success requires treating AI adoption as a comprehensive organizational change, not just a technology acquisition. -->

- **ツール採用 vs. システム変革：** 周囲のシステム（プロセス、役割、文化）が進化していなければ、AIツールを単に展開するだけでは限られた利益しか得られない。多くの失敗したパイロットは、変化していない組織にAIを「プラグイン」しようとすることに起因する。真の利益は、ワークフローがAIの強みを中心に再設計されるときに生まれる。これは、作業の分割方法を変更すること（おそらくAIが取り組める小さなインクリメントに）、イベントのケイデンスを調整すること（例えば、サイクルを加速するためのより頻繁なレビュー）、または説明責任を進化させること（例えば、好奇心旺盛で、多才で、柔軟なプロダクト開発者が監視と設計により多くの時間を費やす）を意味する可能性がある。要するに、成功にはAI採用を単なる技術取得ではなく、包括的な組織変革として扱うことが必要である。

<!-- ### **Implications for Roles** -->

### 役割への影響 {#implications-for-roles}

<!-- **Everyone in the organization will need to adjust in an AI-enhanced Scrum environment:** -->

**AI強化されたスクラム環境では、組織の全員が調整する必要がある：**

<!-- - **Stakeholders, Leaders, and Supporters** ... -->

- **ステークホルダー、リーダー、サポーター**はビジネス側で、コードをより速く書けるからといって、彼らの入力なしに価値がより速くデリバリーされるわけではないことを理解すべきである。AIにより、スクラムチームはおそらくより頻繁に動作するソフトウェアをデリバリーし、ステークホルダーのフィードバックの機会（と必要性）をより多く生み出す。シニアリーダーシップは、コントロールから可能化する行動へとシフトしなければならない - 戦略的ビジョンと明確な境界（例：コンテキスト固有の倫理ガイドラインとAI使用の品質基準）を設定し、その後スクラムチームがそれらの制約内で実行することを信頼する。AIがデリバリーを数週間から数日に加速するとき、従来の官僚主義やステージゲートはボトルネックになる。リーダーはチームが迅速に対応することを妨げる組織的な障害（硬直した承認プロセスや年間予算など）を取り除くことに焦点を当てるべきである。また、信頼と継続的学習の文化を育まなければならない [^15]。これには、チームがミスや未知のことを認めても安全であること（AIとの作業には探索が含まれるため）と、実験を奨励することが含まれる。AI時代の効果的なリーダーシップは、容赦なく価値に焦点を当てながらも高度にエンパワーリングであることを意味する - 方向性とガードレールを設定し、その後チームが迅速にイテレーションできるようにする。リーダーはまた、人間が中心であり続けることを明確に伝えるべきである：AIは人間の創造性とスループットを増強するツールであり、人間の判断に代わるものではない。意味のある目標と目的意識を通じてチームのモチベーションを維持することは依然として不可欠である [^16]。スプリントレビューへの招待と実際の出席は、デジタルプロダクト開発におけるAIの影響と限界のより良い理解を促進できる。

<!-- - The **Product Owner's** role becomes even more critical. ... -->

- **プロダクトオーナー**の役割はさらに重要になる。AIが構築における労働コストを劇的に低下させる（ただし、サブスクリプションやインフラストラクチャなど他のコストは増加する可能性がある）ため、何を構築するか、なぜ構築するかについてのプロダクトオーナーの判断が、チームの成功の主要な要因になることが多い。優れたプロダクトオーナーは、アウトプットよりもアウトカムに焦点を当てる - 各プロダクトバックログアイテムの明確な価値仮説を明確にし、AI構築された機能が実際にその価値をデリバリーするかどうかを厳密に検証する。彼らは迅速な実験に長けていなければならない：AIは最小限の実行可能な機能を素早く生成できるため、数日、数時間、さらには数分で実際のユーザーでアイデアをテストすることが可能である。プロダクトオーナーは、頻繁な実験（A/Bテスト、ベータリリース、レビュー）を実行してデータを収集することでこれを活用すべきである。事実上、プロダクトオーナーはチームのAI能力の認知オーケストレーターとして行動する [^18] - AIに明確な目標、コンテキスト、制約を提供し、その後ユーザー価値のレンズを通じて結果を解釈する。これには強力なプロダクトマネジメントの基礎（顧客への共感、戦略的思考）とAI出力を解釈するための技術的素養が必要である。AIツールとデータ分析について学ぶことに投資するプロダクトオーナー（適切な質問をし、AI駆動のインサイトを調査できるように）は、チームのパフォーマンスを大幅に増幅する。逆に、プロダクトオーナーが弱いか圧倒されている場合、AI対応チームはほとんど価値のない広範な機能を構築する可能性が高い。組織はこれを認識し、それに応じてプロダクトオーナーをサポートすべきである（例：トレーニング、メンタリング、またはコーチングを通じて）。これは、プロダクトオーナーシップの側面をプロダクト開発者に委任（または委譲、意図的であってもスクラムを曲げることになるが）することの重要性が明確になる場所であり、これを可能にするには、信頼を構築するために重要な機能横断的なコラボレーション（例：人間のプロダクト開発者またはエージェント型AIとのアンサンブルワーク）がしばしば必要である。

<!-- - **Scrum Masters** will play a key role ... -->

- **スクラムマスター**は、健全なチームダイナミクスとスクラムの原則を維持しながら、AIの効果的な使用を促進する重要な役割を果たす。彼らはチームがプロセスを調整するのをガイドする必要がある：例えば、「AIツールと自律エージェントは、コード、テスト、ドキュメント、分析、リサーチ、計画、または推奨などの作業を生成または実行する可能性があるが、人間が説明責任を負い続ける。私たちはAIエージェントを積極的に監視し、彼らが許可されていることの明確な境界を定義し、エージェントが合意された制限を超えたり予期しない結果を生成したりするたびに、迅速な手動停止またはオーバーライドメカニズムを配置する」などの新しいワーキングアグリーメントを確立するのを支援する。彼らはAI統合を明示的にカバーするスクラムイベントを促進すべきである。スプリントプランニングでは、これはAIがどのタスクに使用されるかを議論し、AI出力を検証する時間を確保することを意味するかもしれない。レトロスペクティブでは、スクラムマスターはスプリント中にAIがどのように助けたか、または妨げたかをチームに検査させ、改善領域を特定するよう促すことができる。スクラムマスターの役割の重要な部分は、心理的安全性とチームの結束を維持することである。AIツールは不確実性や恐怖（例：役割を心配するプロダクト開発者の間で）を導入する可能性がある。スクラムマスターはこれらのトピックについてオープンな会話を促進し、コンテキスト的に有効な場合にスクラムの価値を強化すべきである。彼らはまた、過度の依存または過少利用を監視する - 例えば、1人のチームメンバーが「AIグル」になり、他のメンバーが離脱している場合、スクラムマスターはスキルを広めるための知識共有やAIとのペアプログラミングを奨励するかもしれない。本質的に、スクラムマスターは彼らが最も得意とすることを続ける - 障害を取り除き、チーム（と組織）をコーチする。

<!-- - For **Product Developers**, AI is a powerful new assistant ... -->

- **プロダクト開発者**にとって、AIは強力な新しいアシスタントである - ただし、監視が必要なものである。プロダクト開発者はAIを活用して定型作業（例：ボイラープレートコードの生成、ユニットテスト/実例による仕様の作成、またはドキュメントのドラフト作成）を自動化し、より複雑で創造的なタスクのための時間を確保すべきである。プロダクト開発者はインクリメントの品質に対して完全に説明責任を負い続ける。AI生成されたコードの各部分は、チームメイトが書いた場合と同じ厳格さでレビューされなければならない。これは、プロダクト開発者が初期コーディングに費やす時間が減り、コードレビュー、テスト、統合に費やす時間が増える可能性があることを意味する。彼らは批判的評価のスキルを磨かなければならない：AI生成出力の微妙なバグ（意味のあるテストハーネスを通じて）、セキュリティ問題、パフォーマンスの落とし穴を特定する。プロダクト開発者は、AI生成コード用の特別なコードレビューチェックリストを確立したり、AIによって導入された重複または非慣用コードを検出するツールを使用したりするかもしれない。さらに、開発者はシステム設計とアーキテクチャの専門知識を維持し深めなければならない。AIはコードを書くのを助けることができるが、一貫したアーキテクチャを自動的に強制することはない - 今のところ、それは依然として人間の責任である。AIとのペアプログラミング（AIをペアパートナーとして扱う）などのプラクティスを採用するチームは、しばしば最良の結果を達成する：AIはソリューションを提案でき、人間の開発者がそれを検証して改善する。重要なことに、開発者は自分自身の学習（言語、フレームワーク、問題ドメイン）に投資し続けるべきである。なぜなら、彼らの幅広い知識によりAIをガイドし、AIができない部分を処理できるからである。一部のチームは、コアスキルと理解が萎縮しないようにするために、AIなしの時折のコーディング演習をスケジュールすることさえある。要約すると、プロダクト開発者の役割は「コードの生成者」から品質と設計のキュレーターへと進化する - 依然として多くのコードを書くが、AIからの貢献をオーケストレーションし、すべてがアウトプット完成の定義とその後のアウトカム完成の定義を満たすことを確保する [^5]。

<!-- AI can create a new tension inside Scrum Teams: a Product Owner can prototype or "vibe code" something in minutes, which can make it feel like the solution is "easy". But turning that prototype into production-ready software (secure, scalable, maintainable, and truly Output Done) can still take weeks or months of real engineering work, even with AI-powered development. AI makes organizational inefficiencies (e.g., silos) more transparent, so organizations need change agents and greater urgency for change more than ever. If this gap stays implicit, expectations collide. Make it explicit with a clear Definition of Output Done and early collaboration between Product Owner and Product Developers. If a Scrum Team cannot deliver value within a Sprint (or a month), there are more fundamental problems to be solved for which AI might not be the first choice. (SGEP/SoftwareEngineeringPractices, SGEP/ProductThinking, SGEP/ScrumExpanded) -->

AIはスクラムチーム内で新しい緊張を生み出す可能性がある：プロダクトオーナーは数分で何かをプロトタイプまたは「バイブコード」でき、ソリューションが「簡単」であるかのように感じさせることができる。しかし、そのプロトタイプをプロダクション対応のソフトウェア（安全で、スケーラブルで、保守可能で、真にアウトプット完成）に変えるには、AI駆動の開発を使用しても、数週間または数ヶ月の実際のエンジニアリング作業がかかる可能性がある。AIは組織の非効率性（例：サイロ）をより透明にするため、組織はこれまで以上にチェンジエージェントと変化への大きな緊急性を必要としている。このギャップが暗黙のままであれば、期待がぶつかる。明確なアウトプット完成の定義とプロダクトオーナーとプロダクト開発者間の早期のコラボレーションで明示的にする。スクラムチームがスプリント（または1ヶ月）内に価値をデリバリーできない場合、AIが最初の選択肢ではないかもしれない、より根本的な問題が解決されるべきである。（SGEP/SoftwareEngineeringPractices、SGEP/ProductThinking、SGEP/ScrumExpanded）

<!-- ### The Continued Importance of Empirical Process Control -->

### 経験的プロセス制御の継続的な重要性 {#the-continued-importance-of-empirical-process-control}

<!-- If Scrum's pillars of transparency, inspection, and adaptation were important before, they are doubly so in the age of AI. AI can generate a flood of output and data that the Scrum Team can drown in or be misled by. It's crucial to make AI activities and results highly visible – for instance, clearly flagging AI-generated work items, sharing the rationale behind AI-driven decisions, and exposing any assumptions the AI made. This transparency enables effective inspection: the Sprint Review might be expanded to not only show what the Scrum Team built, but also how it was built with AI and whether any issues or learnings emerged. By inspecting both the product and the process, the team can catch problems early (e.g., the AI introduced a subtle UX inconsistency, or the team spent too long debugging an AI-written section). With those insights, adaptation follows. Scrum's framework of short Sprints and Sprint Retrospectives is an effective mechanism for iterating on how the Scrum Team uses AI. They can tweak their approach – perhaps adjusting the granularity of tasks given to the AI – and then observe the results in the next Sprint. The key is to treat AI integration as an empirical endeavor: formulate hypotheses about how to use AI effectively, test them on a small scale, review the outcomes, and adapt. Organizations that embrace empirical process control will be able to harness AI to its fullest advantage, steering its power to serve team and customer needs through integrated value streams. Those who abandon an empirical approach (for example, blindly trusting AI outputs or, conversely, dismissing AI after a single failure without learning) risk costly mistakes or missed opportunities. In the end, the heart of Scrum – learning fast and adjusting – is exactly what is needed to thrive in the fast-moving AI era. A continuous adaptive strategy is also required (see the separate strategy document). -->

スクラムの透明性、検査、適応の柱が以前重要であったなら、AIの時代には二重に重要である。AIはスクラムチームが溺れたり誤解させられたりする可能性のあるアウトプットとデータの洪水を生成できる。AIの活動と結果を非常に可視化することが重要である - 例えば、AI生成された作業アイテムを明確にフラグ付けし、AI駆動の意思決定の背後にある根拠を共有し、AIが行った前提を公開する。この透明性は効果的な検査を可能にする：スプリントレビューは、スクラムチームが構築したものだけでなく、AIでどのように構築されたか、問題や学びが生じたかどうかも示すように拡張されるかもしれない。プロダクトとプロセスの両方を検査することで、チームは問題を早期にキャッチできる（例：AIが微妙なUXの不一致を導入した、またはチームがAI作成セクションのデバッグに長時間費やした）。それらの洞察により、適応が続く。スクラムの短いスプリントとスプリントレトロスペクティブのフレームワークは、スクラムチームがAIをどのように使用するかをイテレーションするための効果的なメカニズムである。彼らはアプローチを微調整できる - おそらくAIに与えるタスクの粒度を調整する - そして次のスプリントで結果を観察する。鍵は、AI統合を経験的な取り組みとして扱うことである：AIを効果的に使用する方法についての仮説を立て、小規模でテストし、結果をレビューし、適応する。経験的プロセス制御を受け入れる組織は、AIを最大限に活用し、統合されたバリューストリームを通じてチームと顧客のニーズに奉仕するようにその力を操縦できるようになる。経験的アプローチを放棄する者（例えば、AI出力を盲目的に信頼するか、逆に、学習せずに単一の失敗後にAIを却下する）は、コストのかかるミスや機会の逸失のリスクがある。最終的に、スクラムの心臓部 - 迅速に学習し調整すること - は、まさに急速に動くAI時代に繁栄するために必要なものである。継続的な適応戦略も必要である（別の戦略文書を参照）。

<!-- ## Part 3: Success Patterns of AI Integration -->

## パート3：AI統合の成功パターン {#part-3-success-patterns-of-ai-integration}

<!-- **Organizations** that derive real value from AI share a few key traits [^20]. ... -->

AIから真の価値を引き出す**組織**は、いくつかの主要な特徴を共有している [^20]。彼らはAI統合をローカライズされたツール採用ではなく、システム全体の能力として扱い、エンジニアリングやイノベーションユニット内に孤立させるのではなく、リーダーシップからチームまで、バリューストリーム全体にわたって一貫して組み込む。これらの組織は厳格な品質管理を維持し、AI生成の出力を適切なピアレビューとテストの後にのみ統合し、自動チェック（AIの作業を評価するAIを含む）を使用してコーディングとデリバリー基準を強制する。同時に、より高速なAI駆動の作業がアイデアからアウトカムへの価値の流れを断片化したり中断したりしないようにする。彼らは増加したアウトプットに合わせて検証をスケールし、例えば、AI支援の変更に対して即座に頻繁にユーザーテストを実施したり顧客フィードバックを収集したりする。人間の説明責任は明示的で非交渉可能である：すべてのAIサポートされた結果は人またはチームが所有し、意思決定はAIによって盲目的に行われることはない。文化的に、これらの組織は透明性と学習を促進する - チームはAIがどこで助けるか妨げるかをオープンに議論し、それに応じて働き方を適応させる。最も重要なのは、成功した採用者はアウトカムに焦点を当て続けることである。彼らはデリバリーされた機能の量ではなく、ユーザーとビジネス結果への影響によって成功を測定し、実証的に価値を創造しないAI生成の作業を破棄する意思がある。

<!-- Within **Scrum Teams**, effective patterns include using AI to tighten feedback loops ... -->

**スクラムチーム**内では、効果的なパターンには、フィードバックループを締めるためにAIを使用すること（例：各プロダクト変更を即座に評価するフィードバックループを統合する）と、コンテキスト固有の支援を提供すること（例：AIにプロダクトのドメイン知識や過去のチケットへのアクセスを与えて提案の関連性を向上させる、リトリーバル拡張として知られる技法）が含まれる。ワークフローは、AIが明確に定義された低リスクのタスクを処理し、人間が批判的思考、創造的設計、最終検証に集中するように適応される。ハイパフォーマンスチームはまた、人間のスキルの保持と成長に投資する - 彼らはスクラムチームメンバーが主要なタスクを手動で実行でき、プロダクトドメインを深く理解していることを確保し、AIをガイドし、必要なときに介入できるようにする。一部のチームは、習熟度を鋭く保ち、AI出力が人間の理解と一致することをクロスチェックするために、時折「手動日」を意図的に行う。

<!-- For **Product Owners**, successful AI integration requires tightening—not loosening—the Definition of Output Done regarding quality, and the Definition of Outcome Done for business impact. ... -->

**プロダクトオーナー**にとって、成功するAI統合は、品質に関するアウトプット完成の定義と、ビジネスインパクトに関するアウトカム完成の定義を緩めるのではなく、締めることを必要とする。AIがデリバリーを劇的に加速するにつれて、プロダクトオーナーはより速いアウトプットがより多くの機能ではなく、高品質でより速い学習につながることを確保しなければならない。ハイパフォーマンスのプロダクトオーナーはAI対応のスピードを使用して、仮定をより早くより頻繁に検証する：彼らは明確なアウトカム仮説を定義し、成功がどのように測定されるかを指定し、AI支援の作業が実際のユーザーまたはビジネスインパクトを実証した場合にのみ価値があるとみなされることを確保する。プロダクトバックログアイテムは明示的な問題、受け入れ基準、期待されるアウトカムに基づいており、人間とAIの両方に明確な方向性を提供する。アウトカム完成の定義が主要なステアリングメカニズムになる：この変更が行動、経験、または結果を改善したことを示すエビデンスは何か？測定可能なアウトカム、迅速なフィードバック、針を動かさないAI生成出力を破棄する意思を主張することで、プロダクトオーナーはチームがAI駆動のフィーチャーファクトリーになることを防ぎ、代わりに増加したデリバリースピードを持続的な価値創造に変える。

<!-- For **Product Developers**, successful AI integration depends on strengthening—not relaxing—the Definition of Output Done. ... -->

**プロダクト開発者**にとって、成功するAI統合は、アウトプット完成の定義を緩和するのではなく、強化することに依存する。ハイパフォーマンスチームは、すべてのAI支援の変更が人間が書いた作業と同じ品質基準を満たすことを確保する：統合され、テストされ、レビューされ、リリースしても安全であることが実証されている。AIは、その出力が信頼されて受け入れられることのないジュニアコラボレーターとして扱われる。プロダクト開発者はプロダクトインクリメントの整合性に対して完全に説明責任を負い続ける。実例による仕様（Specification by Example）は「完成」を明示的にする上で中心的な役割を果たす：具体的で実行可能な受け入れ基準とテストはAI支援の実装が始まる前に定義され、人間とAIの両方に明確な参照を提供する。継続的インテグレーション、自動リグレッションテスト、迅速なフィードバックループは、「他のものを壊していないことをどうやって知るか？」という重要な質問に答えることで完成の定義を運用化する。本質的に、これは非常にタイトなテストハーネスを（手動で）作成することを意味する - アーキテクチャ準拠テスト、仕様とアウトカムをガイドする実例による仕様テスト用のPlanguageなど - これはAIによって常に準拠されなければならない（生成AIは少ないものからより多くを作成するため幻覚を起こさなければならず、ギャップを埋めなければならない [^21]）。このようにして、アウトプット完成の定義は、品質、保守性、インクリメントへの信頼を維持しながらAIが開発を加速することを可能にする主要な安全メカニズムになる。

<!-- ## Part 4: Practical Guidance for Implementation -->

## パート4：実装のための実践的ガイダンス {#part-4-practical-guidance-for-implementation}

<!-- **Lay the Groundwork:** ... -->

**基盤を整える：** 安全で効果的なAI使用のための条件を確立することから始める。AIを採用する理由について明確な目標を設定し（例：欠陥率を減少させる、特定のアウトカムのデリバリーを加速する、カスタマーサポートの応答時間を改善する）、これらの目標がすべてのステークホルダーに理解されていることを確保する。基本的なガードレールを開発する：例えば、「AI出力はレビューおよびテストされなければならない」を含むようにアウトプット完成の定義を更新し、AIの初期の許容可能なユースケースを決定する。信頼が構築されるまで、非クリティカルなコンポーネントやテストにはAI生成コードを許可するが、高リスクモジュールには許可しないかもしれない。AIの影響を客観的に測定するためのベースライン指標（例：現在のスループット、経過時間、欠陥密度、顧客満足度スコア）を確立する。重要なのは、チームのトレーニングと実験に事前に投資することである。チームメンバーにサンドボックスでAIツールを試させ、おそらくAIをどのように使用できるかを探索するための内部ハッカソンを実行する。チームが快適で知識があるほど、統合はスムーズになる。

<!-- **Begin with small, contained experiments:** ... -->

**小さく含まれた実験から始める：** ただし、AI採用をポイントソリューションとして扱わない。単一のチームまたはユースケースから始める場合でも、バリューストリーム全体を明示的にトレースする - アイデアと発見から開発、リリース、学習まで。作業が役割、チーム、またはシステム間で引き継がれる場所と、情報が形式を変える場所（例えば、会話からドキュメント、ドキュメントからチケット、チケットからコード、コードからレポート）をマッピングする。これらの引き継ぎとメディアブレークは、遅延、意図の喪失、品質低下が最も頻繁に発生する場所である。これらのポイントで摩擦を減らすためにAIとエージェント型AIを選択的に使用する - 例えば、アーティファクト間で意図を要約し、ツール間でコンテキストを維持し、低リスクの移行を自動化し、要件、実装、アウトカム間の整合性を継続的にチェックする。同時に、すべての意思決定境界で人間をループ内に意図的に保つ。AIは支援、準備、または推奨するかもしれないが、人間は優先順位付け、受け入れ、リリースの決定に対する権限を保持する。目標は最大の自動化ではなく、明確な説明責任を持つ、より統合された、より速い価値の流れである。完全なバリューストリーム全体を最適化しながら小さく始めることで、初期のAI利益が新しいローカル最適化や隠れたボトルネックを作成するのではなく、複利で増加することを確保する。

<!-- **Scale Up What Works:** ... -->

**うまくいくものをスケールアップする：** 最初の問題が解決されたら、パイロットが価値を実証した領域に焦点を当てて、徐々にAIプラクティスをより多くのチームとプロセスに展開する。パイロットチームの学びをブラウンバッグセッションやアンサンブルワークを通じて共有し、他のチームが落とし穴を避けられるようにする。必要に応じて、より良いツールやインフラストラクチャに投資する準備をする - 例えば、AIツールを内部コードリポジトリや知識ベースに接続してより多くのコンテキストを提供する（それによりAI出力の関連性を向上させる）、またはより頻繁なビルドを処理するためにテストインフラストラクチャをアップグレードする。また、経験の浅いチームを「AIチャンピオン」またはパイロットのメンバーとペアリングしてメンタリングすることを検討する。一方、組織全体で測定とフィードバックメカニズムを更新する：AIでより速くデプロイしている場合、変更の影響を迅速に検証するためにユーザーフィードバックループ（分析、サポートフィードバックなど）が加速されていることを確保する。品質指標、サイクルタイム、顧客満足度などの主要な指標を監視し続ける。自動テレメトリとモニタリングアラームを検討する。これらのいずれかがスケールで悪い方向にトレンドし始めた場合、一時停止して根本原因に対処する準備をする（例えば、コードの重複が増加している場合、リファクタリングポリシーを強化するか、自動リントチェックを追加する）。

<!-- **Continuously Adapt:** ... -->

**継続的に適応する：** AI技術は引き続き急速に進化するため、継続的な適応のための能力を構築する。AI使用規範を定期的にレビューする。昨年うまくいったことは、新しいモデルや機能が利用可能になるにつれて改訂が必要になるかもしれない。チームが各スプリントで小さな方法で実験を続けることを奨励し - おそらく新しい種類のタスクにAIツールを試す - 発見を共有する。チームメンバーがAIとの作業に関する観察やヒントを共有できるオープンなコミュニケーションチャネル（例：内部フォーラムやチャットグループ）を維持する。新しいより強力なモデルがリリースされた場合、それを評価する計画を持つ（例：1つのチームに1スプリントでパイロットさせ、報告させる）。同様に、新しいリスク（例：AIがより説得力があるが不正確な出力を生成し始めた場合、プロンプトの明確化や検証などの追加ステップを実装することを検討する）に警戒する。組織のガバナンスを適応可能に保つ。例えば、セキュリティやコンプライアンスのレビュープロセスは、AI生成コンテンツに対処するために進化する必要があるかもしれない。組織レベルでスクラムの検査と適応サイクルまたは組織的なPlan-Do-Study-Actを使用することで、AI統合が停滞しないことを確保する。何よりも、経験的であり続ける：AIが役立っているかどうか、どのように調整するかを決定するためにデータと観察を使用する。おそらくAIは2倍の頻度でリリースすることを可能にする - 顧客価値は実際に増加するか、それとも単に半熟の機能をリリースするだけになるか？それらのアウトカムを監視し、それに応じて戦略を調整する。

<!-- **Common Pitfalls to Avoid:** ... -->

**避けるべき一般的な落とし穴：** 典型的なミスに注意する。AIが熟練した人々に取って代わることができると仮定しない - それはあらゆるステップで人間のガイダンスと監視を依然として必要とする補完物である。一度に多くのことをしようとすることを避ける。プロセスを圧倒する大きなスプラッシュよりも、フィードバックを伴うコントロールされたロールアウトの方が良い。AIのスピードを活用する急ぎで、チームに品質を犠牲にしたりテストをスキップさせたりしない - 今蓄積された技術的負債は、将来の利益をほぼ確実に無効にする。また、虚栄的な指標に対してガードする：チームの速度を倍増させるAIは、追加のアウトプットが低価値であったり、リリースされていないバックログに積み上がったりする場合、逆効果である。真のアウトプット完成の定義（機能するソフトウェアが機能する）とアウトカム完成の定義（価値をデリバリーする）に焦点を当て続けることが重要である。文化的に、失敗した実験を罰しない - 一部のAI使用はうまくいかないだろうし、それは学習曲線の一部である。チームメンバーが非難を恐れると、安全策をとり、AIの潜在能力を決して発見しないだろう。最後に、「分析麻痺」や終わりのないツール比較に陥らない - 実行可能なツールを選び、小さく始め、やりながら学ぶ。この急速に動く分野での最悪のミスは何もしないことである。

<!-- ## Conclusion -->

## 結論 {#conclusion}

<!-- **AI is poised to dramatically reshape how software is developed – and, with it, the fortunes of companies that rely on digital products.** ... -->

**AIはソフトウェアの開発方法を劇的に再形成しようとしている - そしてそれとともに、デジタルプロダクトに依存する企業の運命も。** スクラムにAIをうまく統合する者 - スピードと品質、自動化と人間の判断、アウトプットとアウトカムのバランスを維持する - は、生産性と顧客ニーズへの応答性において飛躍する立場にある。適応に失敗する者は、指数関数的な技術改善の世界で急速に取り残される可能性がある。次の1〜2年は、おそらくAI駆動の未来に必要な能力と文化を構築するための重要な機会の窓を表している [^3]。

<!-- **The evidence suggests that the true differentiator is not who has the most sophisticated AI algorithms, but who can use AI most effectively, integratively, and strategically.** ... -->

**エビデンスは、真の差別化要因は誰が最も洗練されたAIアルゴリズムを持っているかではなく、誰がAIを最も効果的に、統合的に、戦略的に使用できるかであることを示唆している。** スクラムはまさにそれを行うためのフレームワークを提供するが、新しいレベルでスクラムの本質に再コミットすることを必要とする。それは、AIがペースを加速しても、明確な目標、迅速なフィードバック、エンパワーメントされたチームを倍増させることを意味する。この環境では、スクラムチーム全体、特にナビゲーターとしてのプロダクトオーナーの役割 - どの問題を解決するかを決定し、ソリューションが価値をデリバリーすることを確保する - がこれまで以上に重要である。AIが船のスーパーチャージされたエンジンであるなら、プロダクトオーナーは進行方向を提供または共創し、プロダクト開発者は船を運営する。組織はこのプロダクトマネジメント能力に投資しなければならない [^6]。さもなければ、的を外した多くのソフトウェアをより速く構築するリスクがある。

<!-- **In conclusion, integrating AI into Scrum is not a one-time effort but an ongoing process of experimentation and learning.** ... -->

**結論として、AIをスクラムに統合することは一度限りの努力ではなく、実験と学習の継続的なプロセスである。** 技術は変化し続けるだろう。一定でなければならないのは、経験主義、アジリティ、人間中心の思考へのコミットメントである。これを内面化するスクラムチームは、AIを活用して以前は想像できなかったアウトカムを達成し、AI革命を脅威から変革的な機会に変える。始める時は今である - あなたをここまで連れてきた習慣と働き方は、適応し成長し続ける意思がある限り、AIとともに繁栄するのにも役立つだろう。

<!-- ## References -->

## 参考文献 {#references}

[^1]: METR (2025) 'Measuring AI ability to complete long tasks'. Model Evaluation & Threat Research (METR) Blog, 19 March. Available at: [https://metr.org/blog/2025-03-19-measuring-ai-ability-to-complete-long-tasks](https://metr.org/blog/2025-03-19-measuring-ai-ability-to-complete-long-tasks) (Accessed: 19 October 2025).

[^2]: OpenAI (2025) 'Introducing GPT-4.1 in the API'. OpenAI Blog, 14 April. Available at: [https://openai.com/index/gpt-4-1/](https://openai.com/index/gpt-4-1/) (Accessed: 19 October 2025).

[^3]: McKinsey & Company (2025a) 'The state of AI: how organizations are rewiring to capture value'. McKinsey QuantumBlack report, March 2025. Available at: [https://www.mckinsey.com/capabilities/quantumblack/our-insights/the-state-of-ai](https://www.mckinsey.com/capabilities/quantumblack/our-insights/the-state-of-ai) (Accessed: 19 October 2025).

[^4]: McKinsey & Company (2025b) 'AI in the workplace: a report for 2025'. McKinsey Digital, July 2025. Available at: [https://www.mckinsey.com/capabilities/mckinsey-digital/our-insights/superagency-in-the-workplace-empowering-people-to-unlock-ais-full-potential-at-work](https://www.mckinsey.com/capabilities/mckinsey-digital/our-insights/superagency-in-the-workplace-empowering-people-to-unlock-ais-full-potential-at-work) (Accessed: 19 October 2025).

[^5]: Jocham, R., Coleman, J. and Sutherland, J. (2025) *Scrum Guide Expansion Pack*. Available at: [https://scrumexpansion.org](https://scrumexpansion.org) (Accessed: 18 October 2025).

[^6]: Stack Overflow (2025) 'Developers remain willing but reluctant to use AI: the 2025 developer survey results are here'. Stack Overflow Blog, 29 July. Available at: [https://stackoverflow.blog/2025/07/29/developers-remain-willing-but-reluctant-to-use-ai-the-2025-developer-survey-results-are-here/](https://stackoverflow.blog/2025/07/29/developers-remain-willing-but-reluctant-to-use-ai-the-2025-developer-survey-results-are-here/) (Accessed: 4 October 2025).

[^7]: Bender, E.M., Gebru, T., McMillan-Major, A. and Shmitchell, S. (2021) 'On the dangers of stochastic parrots: can language models be too big?', *Proceedings of the 2021 ACM Conference on Fairness, Accountability, and Transparency*, 4(1), pp. 610–623. DOI: 10.1145/3442188.3445922.

[^8]: Qodo AI (2025) *State of AI code quality in 2025*. (Industry report). Available at: [https://www.qodo.ai/reports/state-of-ai-code-quality/](https://www.qodo.ai/reports/state-of-ai-code-quality/) (Accessed: 4 October 2025).

[^9]: GitClear (2024) 'GitClear analyzes 153M lines of code, finds risks of AI'. Arc.dev Talent Blog, 19 June. Available at: [https://arc.dev/talent-blog/impact-of-ai-on-code/](https://arc.dev/talent-blog/impact-of-ai-on-code/) (Accessed: 4 October 2025).

[^10]: GitClear (2025) *AI Copilot code quality: 2025 data suggests 4× growth in code clones*. Available at: [https://www.gitclear.com/ai_assistant_code\_quality\_2025\_research](https://www.gitclear.com/ai_assistant_code\_quality\_2025\_research) (Accessed: 4 October 2025).

[^11]: Gartner (2022) 'Gartner Survey Reveals 80% of Executives Think Automation Can Be Applied to Any Business Decision'. Press release, 22 August 2022. Available at: [https://www.gartner.com/en/newsroom/press-releases/2022-08-22-gartner-survey-reveals-80-percent-of-executives-think-automation-can-be-applied-to-any-business-decision](https://www.gartner.com/en/newsroom/press-releases/2022-08-22-gartner-survey-reveals-80-percent-of-executives-think-automation-can-be-applied-to-any-business-decision) (Accessed: 10 January 2025)

[^12]: Capoot, A. (2025) 'Andrew Ng says the real bottleneck in AI startups isn't coding — it's product management'. Business Insider, 22 August. Available at: [https://www.businessinsider.com/andrew-ng-product-management-bottleneck-coding-ai-startups-2025-8](https://www.businessinsider.com/andrew-ng-product-management-bottleneck-coding-ai-startups-2025-8) (Accessed: 4 October 2025).

[^13]: Parasuraman, R. and Manzey, D.H. (2010) 'Complacency and bias in human use of automation: an attentional integration', *Human Factors*, 52(3), pp. 381–410. DOI: 10.1177/0018720810376055.

[^14]: Mittelstadt, B.D., Allo, P., Taddeo, M., Wachter, S. and Floridi, L. (2016) 'The ethics of algorithms: mapping the debate', *Big Data & Society*, 3(2). DOI: 10.1177/2053951716679679.

[^15]: Edmondson, A.C. (1999) 'Psychological safety and learning behavior in work teams', *Administrative Science Quarterly*, 44(2), pp. 350–383. Available at: [https://doi.org/10.2307/2666999](https://doi.org/10.2307/2666999).

[^16]: Schwartz, B. (2015) *Why we work*. New York: Simon & Schuster.

[^17]: Meira, S., Neves, A. and Braga, C. (2025) 'From programmed labor to meta-cognitive orchestration'. SSRN preprint, 29 June. Available at: [https://ssrn.com/abstract=5329936](https://ssrn.com/abstract=5329936) (Accessed: 19 October 2025).

[^18]: Jocham, R. (2025) 'From passive reviewer to cognitive orchestrator: why AI demands strategic thinking, not administrative tasks'. Scrum.org Blog, 30 November. Available at: [https://www.scrum.org/resources/blog/passive-reviewer-cognitive-orchestrator-why-ai-demands-strategic-thinking-not-administrative-tasks](https://www.scrum.org/resources/blog/passive-reviewer-cognitive-orchestrator-why-ai-demands-strategic-thinking-not-administrative-tasks) (Accessed: 1 December 2025).

[^19]: Deloitte (2020) 'Getting organizational decision making right', Deloitte Insights, 28 February. Available at: [https://www.deloitte.com/us/en/insights/topics/talent/organizational-decision-making.html](https://www.deloitte.com/us/en/insights/topics/talent/organizational-decision-making.html) (Accessed: 14 January 2026).

[^20]: Singh, J. and Sawhney, I. (2026) 'Enterprise-wide AI can unleash the technology's potential: Here's how you get there', World Economic Forum, 16 January. Available at: [https://www.weforum.org/stories/2026/01/enterprise-wide-and-responsible-ai-can-unleash-its-potential-heres-how-you-get-there/](https://www.weforum.org/stories/2026/01/enterprise-wide-and-responsible-ai-can-unleash-its-potential-heres-how-you-get-there/) (Accessed: 17 January 2026).

[^21]: Kalai, A.T., Nachum, O., Vempala, S.S. and Zhang, E. (2025) *Why Language Models Hallucinate*. arXiv. Available at: [https://arxiv.org/abs/2509.04664](https://arxiv.org/abs/2509.04664) (Accessed: 17 January 2026).

---

## 本文書の用語 {#glossary}

共通用語については [スクラムガイド拡張パック用語集](/ja/scrum-guide-expanded/2026.1/#スクラムガイド拡張パック用語集) を参照。

| 英語 | 日本語 | 説明 |
| --- | --- | --- |
| AI-native | AIネイティブ | AIを中核から組み込んで設計・運営される組織 |
| AI-laggard | AI後進 | AI導入が遅れている組織 |
| Automation Bias | 自動化バイアス | 自動化システムを過度に信頼する傾向 |
| Cognitive Orchestrator | 認知オーケストレーター | AIの意図と制約を設定し、アウトカムを調整する役割 |
| Feature Factory | フィーチャーファクトリー | 価値検証なしに機能を大量生産する状態 |
| Generative AI Paradox | 生成AIパラドックス | AI導入率は高いがビジネスインパクトが低い現象 |
| Human-in-the-Loop | ヒューマン・イン・ザ・ループ | AI使用時に人間が監視・意思決定を維持する姿勢 |
| Retrieval Augmentation | リトリーバル拡張 | AIに企業固有の知識を提供して出力の関連性を向上させる技法 |
| Specification by Example (SbE) | 実例による仕様 | 具体例を使って要件を明確化するプラクティス |
| Vibe Code | バイブコード | プロトタイプを素早く作成するカジュアルなコーディング |
