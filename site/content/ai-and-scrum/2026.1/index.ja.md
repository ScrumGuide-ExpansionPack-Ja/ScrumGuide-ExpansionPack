---
# title: AI and Scrum (Expansion of the SGEP)
title: AIとスクラム（SGEP拡張版）
# subtitle: An Evidence-Informed Integration Guide
subtitle: エビデンスに基づく統合ガイド
# description: AI can accelerate delivery, but it can also scale waste if you build the wrong things faster. This guide shows how Scrum's transparency, inspection, and adaptation keeps humans accountable, protects quality, and turns AI-accelerated output into measurable outcomes, with practical guidance for Product Owners, Product Developers, Scrum Masters, and leaders.
description: AIはデリバリーを加速できる。しかし、間違ったものをより速く構築すれば、無駄もまた拡大する。このガイドでは、スクラムの透明性・検査・適応が、いかに人間の説明責任を維持し、品質を守り、AIに加速されたアウトプットを測定可能なアウトカムへと転換するかを、プロダクトオーナー、プロダクト開発者、スクラムマスター、リーダー向けの実践的なガイダンスとともに示す。
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

_本書は、独立した著作物を収録したものである。各セクションは記載の通り、オリジナルのライセンスや著作権状況を保持している。特定の使用権限と要件については、各セクションを参照して欲しい。_

---

<!-- ## Introduction -->

## はじめに {#introduction}

<!-- In the current era of rapid advances in artificial intelligence (AI), integrating AI into Scrum-based digital product development is not just an opportunity but an essential for maintaining relevance and competitiveness. This practical guide is intended for Scrum Teams (including Product Owners, Product Developers, Scrum Masters), and organizational leaders who seek to leverage AI responsibly while upholding Scrum's core principles of empiricism, transparency, and human accountability. It synthesizes the latest research to identify what distinguishes successful AI adopters from those struggling, and provides evidence-based guidance for responsible AI adoption within the Scrum framework. -->

人工知能（AI）が急速に進歩する現代において、AIをスクラムベースのデジタルプロダクト開発に統合することは、単なる機会ではなく、存在意義と競争力を維持するための必須条件となっている。この実践的なガイドは、スクラムの経験主義・透明性・人間の説明責任という中心となる原則を堅持しながら、AIを責任ある形で活用しようとするスクラムチーム（プロダクトオーナー、プロダクト開発者、スクラムマスターを含む）および組織のリーダーを対象としている。最新の研究を統合したうえで、AI導入に成功している組織と苦戦している組織を分ける要因を明らかにし、スクラムフレームワークにおける責任あるAI導入に向けたエビデンスに基づくガイダンスを提供する。

<!-- The urgency of AI integration cannot be overstated. AI systems' ability to autonomously complete complex, extended tasks has been increasing at an exponential rate – roughly doubling every six to seven months [^1]. The competitive landscape has effectively shifted from linear to exponential growth in capabilities [^2]. -->

AI統合の緊急性はいくら強調しても足りない。AIシステムが複雑かつ長期的なタスクを自律的に完了する能力は、指数関数的な速度で増加している - およそ6〜7ヶ月ごとに倍増している [^1]。競争環境は事実上、能力の線形的な成長から指数関数的成長へとシフトした [^2]。

<!-- Industry analyses warn that organizations that delay AI adoption risk strategic obsolescence, as the gap between "AI-native" and "AI-laggard" firms is widening into a structural divide that could lead to mass disruption, consolidation, or even the extinction of slow adopters [^3] [^4]. In short, AI integration is no longer merely an evolution of how we work – it is a race against irrelevance. -->

業界分析は、AI導入に遅れる組織は戦略的陳腐化のリスクに直面すると警告している。「AIネイティブ」企業と「AI後発」企業の間のギャップは、大規模なディスラプションや業界統合、あるいは出遅れた企業の淘汰につながりうる構造的分断へと拡大しつつある [^3] [^4]。要するに、AI統合はもはや単なる働き方の進化ではなく、時代に取り残されないための競争である。

<!-- This guide argues that Scrum's empirical process control and emphasis on human judgment provide a strong foundation for integrating AI responsibly at scale—*provided that organizations also evolve their assurance systems (quality, security, privacy, and auditability), decision rights, and feedback loops to keep pace with AI-driven speed.* -->

このガイドでは、スクラムの経験的プロセス制御と人間の判断の重視が、AIを責任ある形で大規模に統合するための強固な基盤を提供すると主張する - *ただし、組織が保証システム（品質、セキュリティ、プライバシー、トレーサビリティ）、意思決定権、フィードバックループをAIが生み出す速度に追いつくよう進化させることを前提となる。*

<!-- Using the lens of the *Scrum Guide Expansion Pack* [^5] and current AI trends, we illustrate why Scrum is a resilient basis for implementing AI at scale. The SGEP view is that Scrum is mutable (the 2020 Scrum Guide considers it immutable); few noticed this change in June 2025. The SGEP explains the value of each part of Scrum so adopters can adapt with better knowledge. So, here "Scrum" also means adaptations to Scrum that are coherent with the SGEP. -->

*スクラムガイド拡張パック*（SGEP）[^5] と現在のAIトレンドを参照しながら、スクラムがAIを大規模に実装するための堅牢な基盤である理由を論じる。SGEPの立場では、スクラムは適応可能である（2020年版スクラムガイドでは不変とされていた）。この変更はSGEP公開時（2025年6月）にほとんど注目されなかった。SGEPはスクラムの各要素の価値を明示することで、導入者がより深い理解のもとで適応できるよう支援している。したがって、本書における「スクラム」は、SGEPと整合性のあるスクラムの適応形も含む。

<!-- The remainder of this guide is structured as follows. **Part 1 (What We Know)** reviews current evidence on AI's impact on software development. **Part 2 (What This Means)** analyzes the strategic implications of these findings for organizations and teams. **Part 3 (What Good Looks Like)** describes characteristics of successful AI integration observed in practice. Finally, **Part 4 (What To Do)** provides practical implementation guidance, tailored to Scrum roles and organizational readiness. -->

本ガイドの残りの部分は以下のように構成されている。**パート1（現状の把握）**は、ソフトウェア開発に対するAIの影響に関する現在のエビデンスをレビューする。**パート2（これが意味すること）**は、組織とチームに対するこれらの発見の戦略的意味を分析する。**パート3（良い状態とは）**は、実践で観察された成功するAI統合の特徴を説明する。最後に、**パート4（何をすべきか）**は、スクラムの役割と組織の準備状況に合わせた実践的な実装ガイダンスを提供する。

<!-- ## Part 1: What We Know – The Evidence -->

## パート1：現状の把握 - エビデンス {#part-1-what-we-know-the-evidence}

<!-- ### AI's Accelerating Capability Curve -->

### AIの能力向上曲線の加速 {#ais-accelerating-capability-curve}

<!-- The pace of AI improvement has been exponential. In 2023, early general AI models (like GPT-4) could roughly match a junior developer's ability on coding tasks, but often produced as many bugs as they fixed. Extensive human oversight was needed to ensure quality. By 2024, next-generation models (GPT-4.5, Claude 3.5, etc.) were performing more closely to a competent senior developer and generating much cleaner code. These improved capabilities shifted the bottleneck from coding to deciding what to build – teams found the AI could create features faster than the organization could validate their desirability. Strong Product Owners and Product Developers became critical to effectively directing AI efforts. -->

AIの改善ペースは指数関数的である。2023年、初期の汎用AIモデル（GPT-4など）はコーディングタスクにおいてジュニア開発者に匹敵する水準に達していたが、修正したバグと同程度のバグを新たに生み出すことも多かった。品質を確保するには広範な人間によるレビューが必要だった。2024年までに、次世代モデル（GPT-4.5、Claude 3.5など）は有能なシニア開発者により近いパフォーマンスを発揮し、はるかにクリーンなコードを生成するようになった。こうした能力向上により、ボトルネックはコーディングから「何を作るか」の意思決定へとシフトした - チームは、AIが機能を作り出すスピードが、その価値を検証するスピードを上回ることに気づき始めた。AIの取り組みを効果的に方向づけるうえで、優れたプロダクトオーナーとプロダクト開発者の存在が不可欠になった。

<!-- By 2025, frontier models like GPT-5 and Claude 4 achieved expert-level performance. In controlled settings, coding errors became rare; instead, the risk was building the wrong product. The key question became "should we build it (and why)?", rather than "can AI build it?". Product management overtook engineering as the limiting factor in value delivery. Notably, although 78% of companies were using AI by 2025, about 80% reported no significant business impact [^3] [^4] – a "generative AI paradox" attributed to teams producing features without sufficient product guidance or validation. -->

2025年までに、GPT-5やClaude 4などの最先端モデルは専門家レベルのパフォーマンスを達成した。コントロールされた環境では、コーディングエラーは稀になった一方、リスクの本質は、「間違ったプロダクトを作ること」へ移行した。問われるべきは「AIが作れるか？」ではなく「作るべきか、そしてなぜか？」になった。価値提供のボトルネックは、エンジニアリングからプロダクトマネジメントへと移行した。注目すべきことに、2025年時点で企業の78%がAIを活用していたにも関わらず、約80%が有意なビジネスインパクトを報告していない [^3] [^4] - これは十分なプロダクトガイダンスや検証なしに機能を量産してしまうチームにの実態に起因する「生成AIパラドックス」である。

<!-- By 2026 and beyond, AI systems will begin to exceed human expert capabilities in narrow tasks (some models approaching a genius-level). A few leading organizations have redesigned their workflows entirely around AI – in some cases, letting AI agents handle routine tasks – and have started to see exponential performance gains. Meanwhile, the majority still struggle to translate AI into bottom-line value [^3]. By 2027, AI models (e.g., a future GPT-6) may surpass an IQ equivalent of 200, entering superhuman territory. At that point, the challenge will be human comprehension, built-in quality, and control: Product Owners will need to act as cognitive orchestrators, setting intent and constraints for super-intelligent AI and ensuring outcomes align with organizational goals and values [^17] [^18]. In effect, as AI's technical capacity surges, the human ability to steer that capacity toward valuable ends becomes the defining constraint. -->

2026年以降、AIシステムは特定の領域において人間の専門家の能力を超え始める（一部のモデルはすでに天才レベルに迫りつつある）。先進的な組織の一部はワークフロー全体をAI中心に再設計し - 場合によってはAIエージェントに定型タスクを処理させ - 指数関数的なパフォーマンス向上を実現し始めている。一方、大多数の組織は依然としてAIを実質的なビジネス価値に転換できずにいる [^3]。2027年までには、AIモデル（将来のGPT-6など）はIQ換算で200を超え、超人的な領域に踏み込む可能性がある。そうなれば、課題の焦点は「人間の理解力」「品質の組み込み」「制御」になる：プロダクトオーナーは認知オーケストレーター（司令塔）として、超知能AIに対して意図と制約を設定し、アウトカムが組織の目標と価値観に整合していることを確保する役割を担う [^17] [^18]。AIの技術的能力が急伸するにつれ、その能力を価値ある目的へと方向づける人間の能力こそが、決定的な制約となる。

<!-- ### Adoption Reality: Rapid Uptake with Trust Gaps -->

### 導入の現実：急速な普及、信頼にギャップ {#adoption-reality-rapid-uptake-with-trust-gaps}

<!-- AI development tools have seen widespread, rapid adoption among software professionals. By late 2025, an estimated 84% of developers report using AI coding tools in some capacity, with over half using them daily [^6]. Code generation assistants like GitHub Copilot are especially popular, with 63% of professional developers using them [^6]. However, this enthusiastic uptake is tempered by significant issues of trust and reliability. Product Developer confidence in the accuracy of AI outputs has declined as usage increased—surveys show trust in AI-generated code dropped from 69% in 2024 to only 54% in 2025 [^6]. -->

AI開発ツールは、ソフトウェア専門家の間で広範かつ急速に普及している。2025年後半時点で、推定84%の開発者が何らかの形でAIコーディングツールを使用しており、半数以上が毎日活用している [^6]。GitHub Copilotに代表されるコード生成アシスタントは特に人気が高く、プロの開発者の63%が利用している [^6]。しかし、こうした積極的な導入の一方で、信頼性をめぐる深刻な問題が浮かび上がっている。AIのアウトプットの精度に対するプロダクト開発者の信頼は、利用が広がるにつれて低下しており、AI生成コードへの信頼度は2024年の69%から2025年にはわずか54%まで落ち込んだ [^6]。

<!-- The most common frustration is getting solutions that are "almost right, but not quite"—the AI's output appears plausible yet contains subtle errors that create additional work to detect and correct. These findings echo broader concerns about large language models producing fluent but potentially misleading outputs [^7]. In effect, many teams adopt the tools quickly, but then spend substantial time double-checking and correcting AI output. Dave Farley suggests manually creating Specification by Example test harnesses, as the AI cannot be trusted to "mark its own homework"; the specificity of SbE provides the concrete, testable expectations that AI needs to translate qualitative prompts into verifiable behavior. -->

最も多く聞かれる不満は、「ほぼ正しいが、完全ではない」アウトプットへの対応である - AIの出力はもっともらしく見えるが、発見と修正に手間のかかる微妙なエラーを含んでいることが多い。これは、大規模言語モデルが流暢でありながら潜在的に誤解を招きうる出力を生成するという、より広い懸念とも重なる [^7]。結果として多くのチームは、ツールを素早く導入したものの、その後AIのアウトプットの確認と修正にかなりの時間を費やすことになる。Dave Farleyは、AIは「自分の答案を自分で採点する」ことができいとして、実例による仕様（Specification by Example：SbE）のテストハーネスを人間が手動で作成することを推奨している。SbEの具体性は、AIが定性的なプロンプトを検証可能な振る舞いに変換するための、明確でテスト可能な期待値を得ることができる。

<!-- Compounding this is a productivity paradox. On the surface, self-reported productivity is up: 78% of developers using AI report that it makes them more productive [^8]. At the same time, 76% of these developers report they do not fully trust AI-generated code [^8]. In practice, experienced engineers often find that for complex tasks, the overhead of vetting AI-generated output can reduce or even negate productivity gains. One study found that senior developers experienced about a 19% decrease in performance on complicated coding tasks when using an AI assistant, due to the time spent reviewing and testing the AI's work [^8]. In other words, speed gains from AI drafting can be offset by verification costs. Without process changes, AI's promised efficiency risks turning into a situation where developers do two jobs—building software and policing the AI—which is not sustainable. -->

これに加えて生産性パラドックスという問題がある。表面上は自己報告の生産性は上昇している：AIを使用する開発者の78%が「生産性が上がった」と報告している [^8]。しかしその一方で、同じ開発者の76%がAI生成コードを完全には信頼していないとも答えている [^8]。実際には、経験豊富なエンジニアほど、複雑なタスクではAIが生成したアウトプットの検証のオーバーヘッドが生産性向上を相殺、あるいは逆転させうることに気づいている。ある研究では、シニア開発者がAIアシスタントを使用した場合、AIの作業のレビューとテストに費やす時間により、複雑なコーディングタスクのパフォーマンスが約19%低下したことが判明した [^8]。つまり、AIによる作業速度の向上は、検証コストによって相殺される可能性がある。プロセスを見直さない限り、AIがもたらすはずの効率化は、開発者が「ソフトウェアの開発とAIの監視」という二重の役割を担う状況へと変質するリスクがある - これは持続可能な働き方ではない。

<!-- ### Code Quality and Failure Patterns -->

### コード品質と失敗パターン {#code-quality-and-failure-patterns}

<!-- Despite rapid tool adoption at the developer level, scaling AI initiatives to production remains uneven; Gartner (2022) reports that on average, 54% of AI projects make it from pilot to production, implying that a substantial share do not reach production at all [^11]. -->

開発者レベルでのツール導入が急速に進む一方、AIの構想を本番環境へとスケールさせることは依然として容易ではない。Gartner（2022）によれば、AIプロジェクトがパイロットから本番環境へと移行できる割合は平均54%にとどまっており、相当数のプロジェクトが本番稼働に至らないまま終わることを示している [^11]。

<!-- Early evidence from real-world projects suggests that introducing AI into development can degrade code quality if not carefully managed. Analyses of large codebases have found troubling patterns as AI coding assistance became more common. For example, code duplication in some AI-assisted projects increased significantly (from \~8% to \~12% of lines changed), and refactoring activity – developers improving existing code – dropped sharply as teams pumped out new code instead of refining it [^9] [^10]. -->

実世界のプロジェクトからの初期のエビデンスは、適切に管理されなければ、AIの導入がコード品質を低下させる可能性があることを示唆している。AIコーディング支援の普及に伴い、大規模なコードベースの分析から憂慮すべきパターンが明らかになってきた。例えば、AI支援を導入した一部のプロジェクトでは、コードの重複が大幅に増加し（変更された行の約8%から約12%へ）、開発者が既存のコードを改善するリファクタリング活動は急激に減少した。チームがコードを洗練させる代わりに新しいコードを量産するようになったためである [^9] [^10]。

<!-- In 2024, observers noted that, for the first time, copy-pasted or AI-generated code additions exceeded refactored code edits [^10]. This indicates that without deliberate safeguards, AI can tempt teams to prioritize speed over craftsmanship or engineering. The result is accumulating technical debt or a mess – a growing burden of messy, fragile code that may work initially but becomes costly to maintain. In short, AI lets you go faster, but if that speed comes without improved practices, you simply accelerate the rate at which your codebase becomes complex and error-prone. -->

2024年には、コピー&ペーストまたはAI生成によるコードの追加が、リファクタリングによるコードの修正を初めて上回った [^10]。これは、意図的なセーフガードがなければ、AIがチームにエンジニアリングの品質よりもスピードを優先させる誘因になりうることを示している。その結果として蓄積されるのが技術的負債、すなわち将来の混乱の種である。当初は動作するかもしれないが、時間とともに維持コストが膨らむ、雑然として脆いコードが積み重なっていく。要するに、AIは開発速度を高めてくれる。しかし、プラクティスの改善を伴わないスピードアップは、コードベースの複雑化とエラーの頻発を加速させるだけである。

<!-- Common causes include treating AI as a superficial add-on rather than redesigning workflows; a lack of supporting processes (such as robust testing and validation of AI outputs); organizational resistance to the changes in roles and habits AI necessitates; and a mismatch between fast AI-driven development and slower legacy release or feedback processes. The net effect is a two-speed IT reality: many organizations accelerate development with AI only to hit bottlenecks in quality assurance, user testing, or stakeholder review. -->

主な原因としては、次の四点が挙げられる。ワークフローを抜本的に再設計するのではなくAIを表面的な付け足しとして扱うこと、AIのアウトプットに対する堅牢なテストや検証といった支援プロセスの欠如、AIが求める役割と習慣の変化に対する組織的な抵抗、そしてAI駆動開発のスピードとレガシーなリリース・フィードバックプロセスの遅さとのミスマッチである。その結果として生じるのが「二つの速度のIT」という現実である：AIで開発を加速しても、品質保証・ユーザーテスト・ステークホルダーレビューでボトルネックに突き当たる組織が後を絶たない。

<!-- Only a small elite has managed to align their entire system (people, processes, and technology) to capitalize on AI fully. These high performers build closed-loop feedback into their AI workflows (catching errors early with automated checks), give AI tools rich context (e.g., company-specific training data) to improve relevance, and redesign roles and norms to make AI a core part of the process rather than a novelty. Such organizations report substantial productivity gains while maintaining quality, whereas the rest see at best modest gains offset by new challenges [^8]. -->

システム全体（人・プロセス・テクノロジー）をAI活用に向けて一体的に整合させることに成功した組織は、まだ一握りにすぎない。こうしたハイパフォーマーに共通するのは三つの取り組みである。第一に、自動チェックでエラーを検出・修正するクローズドループのフィードバックをAIワークフローに組み込むこと。第二に、企業固有の学習データなど豊富なコンテキストをAIツールに提供して精度を高めること。第三に、AIを一時的な目新しさとしてではなくプロセスの中核に据えるべく、役割と規範を再設計することである。こうした組織は品質を維持しながら大幅な生産性向上を実現している。一方、大多数の組織では、わずかな改善が新たな課題によって相殺されるのがせいぜいという状況にとどまっている [^8]。

<!-- ## Part 2: What This Means – Strategic Implications -->

## パート2：これが意味すること - 戦略的意味 {#part-2-what-this-means-strategic-implications}

<!-- **AI's impact on Scrum Teams creates a fundamental paradox:** it accelerates output but does not automatically guarantee outcomes. To convert increased development speed into real customer value, organizations must evolve not only their technical practices but also their management and product strategies—especially how decisions are made. In an AI-accelerated environment, centralized approval chains and slow, hierarchical prioritization become bottlenecks; value requires distributed decision making within clear strategic guardrails, so teams can quickly choose, test, and adapt based on evidence rather than waiting for permission. -->

**スクラムチームに対するAIの影響は、根本的なパラドックスを生み出す：** アウトプットは加速するが、アウトカムが自動的に保証されるわけではない。高まった開発スピードを実際の顧客価値へと転換するには、技術的プラクティスだけでなく、マネジメントやプロダクト戦略 — 特に意思決定の方法 — も進化させなければならない。AIによって加速された環境においては、中央集権的な承認のチェーンや遅い階層的な優先順位付けはボトルネックとなる。価値を生み出すには、明確な戦略的ガードレールのもとで意思決定を分散させ、チームが許可を待つのではなくエビデンスに基づいて迅速に選択・テスト・適応できる状態が求められる。

<!-- **Speed without Direction:** The chief risk is that AI enables the wrong things to be built faster. Without a strong Product Goal and fast feedback loops, teams can become high-throughput "feature factories," producing lots of features that do not solve real problems [^12]. The presence of AI magnifies strengths and weaknesses. If your Scrum practice is sound (empirically guided, rhythmic in a direction of travel, professional, disciplined, psychologically safe, and value-focused), AI can amplify its effectiveness; if your process lacks clear direction or quality discipline, AI will amplify the dysfunction. As one observer noted, if you have a broken compass, running faster just gets you lost more quickly. -->

**方向性のないスピード:** 最大のリスクは、AIによって「間違ったもの」がより速く作られてしまうことである。強固なプロダクトゴールと迅速なフィードバックループがなければ、チームは高スループットの「フィーチャーファクトリー」と化し、実際の問題を解決しない機能を大量に生産しかねない [^12]。AIの存在は、強みも弱みも等しく増幅する。スクラムプラクティスが健全（経験主義に則り、目的に向かってリズムを持ち、プロフェッショナルで、規律があり、心理的安全性が確保され、価値に焦点を合わせている）であれば、AIはその効果をさらに高める。一方、プロセスに明確な方向性や品質への規律が欠けていれば、AIは機能不全をも増幅する。ある観察者が指摘したように、壊れたコンパスを持って速く走れば、より早く迷子になるだけである。

<!-- Many organizations have historically optimized for ease of management—predictability, reporting, centralized control, and approval structures—rather than ease of delivery. AI acts as a magnifying glass on this imbalance. When work is optimized for managerial convenience rather than fast learning and delivery, AI does not fix the system; it accelerates local output while amplifying systemic dysfunction. In such environments, AI enables teams to build the wrong things faster, increasing waste rather than value. -->

多くの組織はこれまで、デリバリーのしやすさよりもマネジメントのしやすさ — 予測可能性、レポーティング、中央集権的な管理、承認プロセス — に最適化されてきた。AIはこの不均衡を映し出す拡大鏡である。迅速な学習やデリバリーではなく管理上の都合に最適化された環境では、AIがシステムの問題を解消することはない。局所的なアウトプットを加速する一方で、システム全体の機能不全を増幅させるだけである。結果として、AIはチームが間違ったものをより速く作ることを助長し、価値ではなく無駄を増加させる。

<!-- **Exponential Change, Short Window:** As AI capabilities improve at an exponential rate and are rapidly adopted across industries, organizations face a narrow window to adapt. Practically, experts suggest that companies have about 12–24 months to achieve meaningful AI integration before falling too far behind [^3]. This is not hyperbole; it reflects exponential curves: a few months' delay now could translate into years behind a competitor that is compounding its learning and capabilities. Market trends already show early adopters pulling ahead via network effects and data advantages that latecomers will struggle to catch up to [^4]. The implication is clear – a sense of urgency must permeate the delivery of outcomes in a direction. AI adoption is no longer a "wait and see" proposition; it's adapt soon or risk irrelevance. -->

**指数関数的な変化と残された短い猶予：** AIの能力は指数関数的に向上し、あらゆる業界で急速に普及している。組織が適応できる時間的猶予は限られている。専門家によれば、企業が取り残される前に実質的なAI統合を実現するには、残された期間は約12〜24ヶ月とされる [^3]。これは誇張ではなく、指数曲線の現実を反映している。現時点での数ヶ月の遅れが、学習と能力を着実に積み重ねている競合他社に対して数年分の差に広がりかねない。市場トレンドはすでに、ネットワーク効果とデータ優位性によってアーリーアダプターがリードを広げ、後発者が追いつくことが困難になりつつある現実を示している [^4]。結論は明白である — 方向性を持ったアウトカムのデリバリーに、切迫感が不可欠である。AI導入は、もはや「様子見」で済む段階ではない。すぐに適応するか、時代に取り残されるかの二択である。

<!-- ### **Key Tensions to Manage** -->

### 管理すべき主要な緊張関係 {#key-tensions-to-manage}

<!-- **In pursuing AI integration, organizations must deliberately balance several inherent tensions:** -->

**AI統合を推進するにあたり、組織はいくつかの固有の緊張関係を意識的に調整しなければならない：**

<!-- - **Structure vs. Agency:** AI accelerates speed and thereby the need for cross-functional collaboration, and the feasibility of distributed decision-making. Traditional hierarchical organization structures (organization charts, functional silos, centralized approvals) might still matter for legal accountability and people management—but they often become poor representations of how value is created and how decisions flow [^19]. If the organization relies solely on the hierarchy to coordinate work, AI will simply accelerate local output while amplifying enterprise bottlenecks (handoffs, queues, approvals). Managing this tension means keeping the org chart as the accountability skeleton while operating day to day through value streams, clear decision rights, and empowered teams. Leaders must define strategic intent and guardrails (risk, compliance, quality, context-specific ethics), then deliberately push decision authority to the lowest responsible level so teams can act, learn, and adapt quickly based on evidence. -->

**構造 vs. 主体性：** AIは業務のスピードを高め、それに伴い機能横断的なコラボレーションの必要性と分散型意思決定の実現可能性も増す。伝統的な階層型組織構造（組織図、機能別サイロ、中央集権的承認）は、法的説明責任や人材管理のうえでは依然として重要かもしれない。しかし、価値がどのように創造され、意思決定がどのように流れるかという実態を正しく反映できないことが多い [^19]。組織が仕事の調整を階層構造だけに頼っている場合、AIは組織全体のボトルネック（引き継ぎ、キュー、承認）を増幅しつつ、局所的なアウトプットを加速するにとどまる。この緊張に対処するには、組織図を説明責任の骨格として維持しながら、日常の業務をバリューストリーム、明確な意思決定権、権限を持つチームを通じて運営する必要がある。リーダーは戦略的意図とガードレール（リスク、コンプライアンス、品質、文脈に応じた倫理基準）を定め、チームがエビデンスに基づいて迅速に行動・学習・適応できるよう、意思決定権限を現場に最も近い責任を持つ階層まで委譲しなければならない。

<!-- - **Speed vs. Quality**: AI can dramatically accelerate development, but moving faster can compromise quality unless active measures are taken. Without guardrails, teams accumulate technical debt faster than they can pay it down. Declining code quality has already been observed in some AI-adopting teams [^10]. Managing this tension means investing in automated testing, refactoring, and a stricter Definition of Output Done to keep quality constant even as velocity increases. Leadership must send the message that quality is not negotiable – speed is beneficial only if you can maintain quality. -->

- **スピード vs. 品質：** AIは開発を劇的に加速できる。しかし、適切な対策を講じなければ、スピードの向上は品質の犠牲を伴いかねない。ガードレールがなければ、チームは返済のペースを上回る速さで技術的負債を積み上げてしまう。こうした品質の低下は、AI導入チームの一部ですでに観察されている [^10]。この緊張に対処するには、開発速度が上がっても品質を維持できるよう、自動テスト、リファクタリング、より厳格なアウトプット完成の定義への投資が求められる。リーダーシップは、品質は譲れないという姿勢を明確に示さなければならない — スピードは品質を維持できてこそ意味がある。

<!-- - **Automation vs. Accountability**: As AI automates more tasks, human team members may feel less ownership of outcomes. The attitude "the AI suggested it, so we implemented it" can lead to diffused responsibility. This is dangerous because it undermines learning and accountability. To address this, teams should make it clear that AI is a tool and that humans remain accountable for decisions and results. Research on human–automation interaction warns of automation bias and complacency – people may over-trust automated systems and become passive in oversight [^13] [^14]. Scrum Teams must consciously keep a human-in-the-loop attitude: AI may recommend, but humans decide. -->

- **自動化 vs. 説明責任：** AIが自動化するタスクが増えるにつれ、チームメンバーはアウトカムに対するオーナーシップを持ちにくくなる恐れがある。「AIが提案したから実装した」という態度は、責任の所在をあいまいにしかねない。これは学習と説明責任の双方を損なうため危険である。これに対処するには、AIはあくまでもツールであり、意思決定と結果への説明責任は人間が負い続けるという原則をチーム内で明確にすべきである。人間と自動化の相互作用に関する研究は、自動化バイアスと慢心のリスクを指摘している — 人々は自動化されたシステムを過信し、監視の姿勢が受動的になりやすいというものである [^13] [^14]。スクラムチームは、意識的にヒューマン・イン・ザ・ループの姿勢を堅持しなければならない：AIは推奨するかもしれないが、決定は人間がする。

<!-- - **Outputs vs. Outcomes**: AI makes it easy to measure outputs (e.g., lines of code generated, features delivered), but organizations must resist the urge to be activity- or output-driven and remain outcome-driven. The objective measure of success is whether those AI-accelerated outputs provide valuable outcomes for users and business impact. This means doubling down on practices such as defining clear Product Goals, defining feature success metrics, and using hypothesis-driven development. It may be tempting to celebrate how many Product Backlog items an AI completes, but Scrum teams should instead ask, "What measurable benefit did this deliver?" to ensure they are not just doing more busy work faster. -->

- **アウトプット vs. アウトカム：** AIはアウトプット（例：生成されたコード行数、デリバリーされた機能）を測定することを容易にするが、組織は活動やアウトプット駆動になる衝動に抵抗し、アウトカム駆動であり続けなければならない。成功の客観的な尺度は、それらのAI加速されたアウトプットがユーザーに価値あるアウトカムとビジネスインパクトを提供するかどうかである。これは、明確なプロダクトゴールの定義、機能の成功指標の定義、仮説駆動開発の使用などのプラクティスを倍増させることを意味する。AIが完了したプロダクトバックログアイテムの数を祝いたくなるかもしれないが、スクラムチームは代わりに「これは何の測定可能な利益をデリバリーしたか？」と問い、単により多くの忙しい仕事をより速くやっているだけではないことを確認すべきである。

**アウトプット vs. アウトカム：** AIはアウトプット（例：生成コード行数、デリバリーされた機能）の測定を容易にする。しかし組織は、アウトプットの量や活動量で成果を測ろうとする衝動に抗い、アウトカム駆動であり続けなければならない。成功の客観的な尺度は、AIによって加速されたアウトプットが、ユーザーにとって価値あるアウトカムやビジネスインパクトを実際にもたらしているかどうかである。そのためには、明確なプロダクトゴールの設定、機能ごとの成功指標の定義、仮説駆動開発の活用といったプラクティスをいっそう強化する必要がある。AIが完了したプロダクトバックログアイテムの数を誇りたくなるかもしれないが、スクラムチームはむしろ「これはどのような測定できる具体的な効果をもたらしたか？」と問い、単に作業量を加速させているだけではないことを確認すべきである。

<!-- - **Tool Adoption vs. System Transformation**: Simply rolling out AI tools will yield limited benefit if the surrounding system (process, roles, culture) has not evolved. Many failed pilots stem from trying to "plug in" AI to an unchanged organization. Real gains come when workflows are redesigned around AI's strengths. This could mean changing how work is sliced (perhaps into smaller increments that AI can tackle), adjusting event cadences (for example, more frequent reviews to accelerate cycles), or evolving accountabilities (for example, curious, rounded, and flexible Product Developers spending more time on oversight and design). In short, success requires treating AI adoption as a comprehensive organizational change, not just a technology acquisition. -->

**ツール採用 vs. システム変革：** 周囲のシステム（プロセス、役割、文化）が進化しなければ、AIツールを導入するだけでは得られる効果は限定的である。パイロットの多くが失敗するのは、既存の組織を変えないままAIを「後付け」しようとするためである。真の効果は、AIの強みに合わせてワークフロー自体を再設計したときに生まれる。具体的には、作業をAIが処理しやすい小さなインクリメントに分割すること、イベントのケイデンスを調整すること（例：レビューの頻度を上げてサイクルを加速させる）、あるいは説明責任のあり方を見直すこと（例：好奇心旺盛で多才かつ柔軟なプロダクト開発者が、AIによるコード生成を前提に、自らの時間をレビュー・監視・設計へとシフトさせる）などが考えられる。要するに、AI導入の成功には、単なる技術導入ではなく包括的な組織変革として臨むことが欠かせない。

<!-- ### **Implications for Roles** -->

### 役割への影響 {#implications-for-roles}

<!-- **Everyone in the organization will need to adjust in an AI-enhanced Scrum environment:** -->

**AIを活用したスクラム環境では、組織の全員が自らの役割や働き方を見直す必要がある：**

<!-- - **Stakeholders, Leaders, and Supporters** on the business side should understand that just because code can be written faster doesn't mean value is delivered faster without their input. With AI, the Scrum Team will likely deliver working software more frequently, creating more opportunities (and a greater need) for stakeholder feedback. Senior leadership must shift from controlling to enabling behavior – setting strategic vision and clear boundaries (e.g., context-specific ethical guidelines and quality standards for AI use)- and then trusting Scrum Teams to execute within those constraints. Traditional bureaucracy or stage-gates will become bottlenecks when AI accelerates delivery from weeks to days. Leaders should focus on removing organizational impediments (like rigid approval processes or annual budgets) that prevent teams from responding quickly. They also must foster a culture of trust and continuous learning [^15]. This includes making it safe for teams to admit mistakes or unknowns (since working with AI involves exploration) and encouraging experimentation. Effective leadership in the AI era means being ruthlessly value-focused yet highly empowering – set the direction and guardrails, then let the teams iterate rapidly. Leaders should also clearly communicate that people remain central: AI is a tool to augment human creativity and throughput, not a replacement for human judgment. Keeping teams motivated through meaningful goals and a sense of purpose remains essential [^16]. Invitations and actually attending to Sprint Reviews could foster a better understanding of the impact and limitations of AI in digital product development. -->

- ビジネス側の**ステークホルダー、リーダー、サポーター**は、コードをより速く書けるようになったからといって、自分たちの関与なしに価値が速くデリバリーされるわけではないことを理解すべきである。AIを活用することで、スクラムチームは動くソフトウェアをより頻繁にデリバリーするようになり、ステークホルダーからのフィードバックを受ける機会も必要性も増す。シニアリーダーシップは、コントロールから支援へとふるまいを変えなければならない — 戦略的ビジョンと明確な境界（例：状況に応じた倫理ガイドラインやAI使用の品質基準）を設定した上で、スクラムチームがその制約内で実行することを信頼する。AIがデリバリーのリードタイムを数週間から数日に短縮するとき、従来の官僚的プロセスやステージゲートはボトルネックとなる。リーダーは、チームの迅速な対応を阻む組織的障害（硬直した承認プロセスや年間予算など）の除去に注力すべきである。加えて、信頼と継続的学習の文化を醸成しなければならない [^15]。これには、チームがミスや不明点を安心して共有できる環境をつくること（AIとの協働には試行錯誤が伴うため）、そして実験を奨励することが含まれる。AI時代に求められるリーダーシップとは、価値への徹底したフォーカスと、チームへの高度な権限移譲を両立させることである — 方向性とガードレールを示し、あとはチームが迅速にイテレーションできるようにする。また、人間が依然として中心的存在であることを明確に発信すべきである：AIは人間の創造性と生産性を増強するツールであり、人間の判断に取って代わるものではない。意味のある目標と目的意識を通じてチームのモチベーションを維持することは、引き続き不可欠である [^16]。スプリントレビューへの招待と積極的な参加は、デジタルプロダクト開発におけるAIの可能性と限界をより深く理解することにつながる。

<!-- - The **Product Owner's** role becomes even more critical. With AI dramatically lowering labour costs in building (but potentially increasing other costs, such as subscriptions or infrastructure), the Product Owner's judgment about what to build and why is now often the primary factor in a team's success. Great Product Owners will focus on outcomes over outputs – articulating clear value hypotheses for each Product Backlog item and rigorously validating whether AI-built features actually deliver that value. They must become adept at rapid experimentation: since AI can churn out a minimum viable feature quickly, it's feasible to test an idea with real users in days, hours, or even minutes. The Product Owner should leverage this by running frequent experiments (A/B tests, beta releases, reviews) to gather data. In effect, the Product Owner acts as a cognitive orchestrator for the team's AI capabilities [^18] – providing the AI with clear goals, context, and constraints, then interpreting the results through the lens of user value. This requires strong product management fundamentals (customer empathy, strategic thinking) and technical acumen to interpret AI outputs. Product Owners who invest in learning about AI tools and data analytics (so they can ask the right questions and probe AI-driven insights) will significantly amplify their team's performance. Conversely, if the Product Owner is weak or overwhelmed, an AI-enabled team is likely to build extensive functionality with little value. Organizations should recognize this and support their Product Owners accordingly (e.g., through training, mentoring, or coaching). This is where the importance of delegating (or devolving, even if doing so bends Scrum, albeit intentionally) aspects of product ownership to Product Developers becomes clear, and enabling this often requires cross-functional collaboration (e.g., ensemble work with human Product Developers or agentic-AI) that is crucial to building trust. -->

- **プロダクトオーナー**の役割はさらに重要性を増す。AIが開発における労働コストを劇的に引き下げる一方（サブスクリプションやインフラストラクチャなど別のコストが増加する可能性はある）、何を構築するか、なぜ構築するかについてのプロダクトオーナーの判断が、チームの成功を左右する最大の要因となることが多い。優れたプロダクトオーナーはアウトプットよりもアウトカムに注力する — 各プロダクトバックログアイテムに対して明確な価値仮説を立て、AIで構築した機能が実際にその価値をもたらしているかを厳密に検証する。迅速な実験にも長けている必要がある：AIは実用最小限の機能を素早く生み出せるため、数日、数時間、あるいは数分で実際のユーザーを相手にアイデアを検証できる。プロダクトオーナーは頻繁な実験（A/Bテスト、ベータリリース、レビュー）を通じてデータを収集し、この利点を活かすべきである。実質的に、プロダクトオーナーはチームのAI活用の認知オーケストレーター（司令塔）として機能する [^18] — AIに明確な目標・コンテキスト・制約を与え、得られた結果をユーザー価値の観点から解釈する。これには堅実なプロダクトマネジメントの基礎（顧客への共感、戦略的思考）と、AIのアウトプットを評価できる技術的素養が求められる。AIツールやデータ分析を学ぶことに投資し、的確な問いを立ててAI由来のインサイトを深掘りできるプロダクトオーナーは、チームのパフォーマンスを大きく引き上げる。一方で、プロダクトオーナーの力量が不足していたり余裕を失っていたりすると、AI活用チームは価値の乏しい機能を大量に生み出しかねない。組織はこの点を認識し、トレーニング、メンタリング、コーチングなどを通じてプロダクトオーナーを支援すべきである。ここで明らかになるのが、プロダクトオーナーシップの一部をプロダクト開発者に委任（または委譲、意図的であってもスクラムを曲げることになるが）することの重要性であり、それを実現するには信頼の構築に不可欠な機能横断的コラボレーション（例：人間のプロダクト開発者やエージェント型AIとのチーム一体での協働）が求められることが多い。

<!-- - **Scrum Masters** will play a key role in facilitating the effective use of AI while preserving healthy team dynamics and Scrum principles. They will need to guide the team in adjusting its processes: for instance, helping establish new working agreements such as "AI tools and autonomous agents may generate or perform work such as code, tests, documentation, analysis, research, planning, or recommendations, but humans remain accountable. We actively monitor AI agents, define clear boundaries for what they are allowed to do, and put fast manual stop or override mechanisms in place whenever an agent goes beyond agreed limits or produces unexpected results." They should foster Scrum events explicitly covering AI integration. In Sprint Planning, this might mean discussing which tasks the AI will be used for and setting aside time to validate AI outputs. In Retrospectives, the Scrum Master can prompt the team to inspect how AI helped or hindered during the Sprint and identify areas for improvement. A critical part of the Scrum Master's role is maintaining psychological safety and team cohesion. AI tools may introduce uncertainty or even fear (e.g., among Product Developers who worry about their role). The Scrum Master should facilitate open conversations about these topics and reinforce the Scrum values when they are contextually valid. They also keep an eye on over-reliance or under-utilization – for example, if one team member becomes the "AI guru" and others disengage, the Scrum Master might encourage knowledge sharing or pair programming with AI to spread skills. Essentially, Scrum Masters continue to do what they do best – remove impediments and coach the team (and the organization). -->

- **スクラムマスター**は、健全なチームダイナミクスとスクラムの原則を守りつつ、AIの効果的な活用を促進する上で鍵となる役割を担う。チームがプロセスを適応させていく際の導き手となる必要がある：例えば、「AIツールや自律エージェントはコード、テスト、ドキュメント、分析、リサーチ、計画、推奨事項などの作業を生成・実行する場合があるが、説明責任は人間が負い続ける。AIエージェントを積極的に監視し、その行動範囲に明確な境界を設け、合意した制限を超えたり想定外の結果を出した場合には、速やかに手動で停止・修正できる仕組みを整える」といった新たなワーキングアグリーメントの策定を支援する。AI活用を明示的に扱うスクラムイベントの運営も促すべきである。スプリントプランニングでは、どのタスクにAIを使うかを議論し、AIのアウトプットを検証するための時間を確保する。レトロスペクティブでは、スプリント中にAIがどう役立ち、どこで障害になったかをチームに振り返らせ、改善点を特定するよう促す。スクラムマスターの役割で特に重要なのは、心理的安全性とチームの結束の維持である。AIツールは不確実性や不安（例：自身の役割を心配するプロダクト開発者の懸念）をもたらしうる。スクラムマスターはこうしたテーマについてオープンな対話を促し、状況に応じてスクラムの価値を補強すべきである。過剰な依存や過少な活用にも目を配る必要がある—例えば、特定のメンバーだけが「AIの達人」となり他のメンバーが消極的になっている場合、知識共有やAIとのペアプログラミングを通じてスキルの平準化を促すとよい。つまるところ、スクラムマスターは自身の最も得意とすることを引き続き行う — 障害の除去と、チーム（そして組織）のコーチングである。

<!-- - For **Product Developers**, AI is a powerful new assistant – but one that requires oversight. Product Developers should leverage AI to automate rote work (e.g., generating boilerplate code, writing unit tests/specification by example, or producing documentation drafts), freeing up time for more complex and creative tasks. Product Developers remain fully accountable for the quality of the increment. Every piece of AI-generated code must be reviewed with the same rigor as if a teammate wrote it. This means Product Developers may spend less time on initial coding and more on code review, testing, and integration. They must sharpen their skills in critical evaluation: identifying subtle bugs (through a meaningful test harness), security issues, and performance pitfalls in AI-generated output. Product Developers might establish special code review checklists for AI-generated code or use tools to detect duplicative or non-idiomatic code introduced by AI. Additionally, developers need to maintain and deepen their expertise in system design and architecture. AI can help write code, but it won't automatically enforce a coherent architecture – for now, that is still a human responsibility. Teams that embrace practices such as pair programming with AI (treating the AI as a pair partner) often achieve the best results: the AI can propose solutions, and a human developer vets and improves them. Importantly, developers should continue investing in their own learning (languages, frameworks, problem domains) because their broad knowledge enables them to guide the AI and handle the parts the AI cannot. Some teams even schedule occasional coding exercises without AI to ensure core skills and understanding don't atrophy. In summary, the Product Developer role evolves from "generator of code" to a curator of quality and design – still writing plenty of code, but also orchestrating contributions from AI and ensuring everything meets the Definition of Output Done and the subsequent Definition of Outcome Done [^5]. -->

- **プロダクト開発者**にとって、AIは強力な新しいアシスタントである — ただし、適切な監視を伴うものである。プロダクト開発者はAIを活用して定型作業（例：定型コード（ボイラープレート）の生成、ユニットテスト/実例による仕様（SbE）の作成、ドキュメントのドラフト作成）を自動化し、より複雑で創造的な作業に時間を充てるべきである。インクリメントの品質に対する完全な説明責任はプロダクト開発者にあり続ける。AIが生成したコードはすべて、チームメイトが書いたものと同じ厳格さでレビューしなければならない。結果として、初期コーディングに費やす時間が減り、コードレビュー、テスト、統合に費やす時間が増えることになるだろう。批判的に評価するスキルを磨くことも求められる：AIが生成するアウトプットに含まれる微妙なバグ（有意義なテストハーネスの活用が鍵となる）、セキュリティ上の問題、パフォーマンスの落とし穴を見抜く力である。AI生成コード専用のコードレビューチェックリストを設けたり、AIが持ち込む冗長なコードや不自然な書き方を検出するツールを活用したりすることも考えられる。加えて、システム設計やアーキテクチャに関する専門性を維持し、さらに深める必要がある。AIはコードの作成を支援できるが、一貫性のあるアーキテクチャを自律的に維持することは今のところできない — それは依然として人間の責務である。AIとのペアプログラミング（AIをペアパートナーとして扱う）を取り入れるチームは、最良の結果を得ることが多い：AIが解決策を提案し、人間の開発者がそれを精査・改善するという形である。開発者が自身の学習（言語、フレームワーク、問題ドメイン）への投資を続けることも重要である。幅広い知識があってこそAIを適切に導き、AIでは対応できない部分を担えるからである。コアスキルや理解力が衰えないよう、あえてAIに頼らないコーディング演習を定期的に行うチームもある。要するに、プロダクト開発者の役割は「コードの生成者」から品質と設計のキュレーターへと進化する — 依然として多くのコードを書くが、同時にAIからの成果物をまとめ上げ、すべてがアウトプット完成の定義、さらにはアウトカム完成の定義を満たすことを責任を持って確認する [^5]。

<!-- AI can create a new tension inside Scrum Teams: a Product Owner can prototype or "vibe code" something in minutes, which can make it feel like the solution is "easy". But turning that prototype into production-ready software (secure, scalable, maintainable, and truly Output Done) can still take weeks or months of real engineering work, even with AI-powered development. AI makes organizational inefficiencies (e.g., silos) more transparent, so organizations need change agents and greater urgency for change more than ever. If this gap stays implicit, expectations collide. Make it explicit with a clear Definition of Output Done and early collaboration between Product Owner and Product Developers. If a Scrum Team cannot deliver value within a Sprint (or a month), there are more fundamental problems to be solved for which AI might not be the first choice. (SGEP/SoftwareEngineeringPractices, SGEP/ProductThinking, SGEP/ScrumExpanded) -->

AIはスクラムチーム内に新たな緊張をもたらす可能性がある：プロダクトオーナーが数分でプロトタイピングや「バイブコード」で形にできるため、ソリューションが「簡単」に見えてしまうことがある。しかし、そのプロトタイプをプロダクション対応のソフトウェア（安全で、スケーラブルで、保守可能で、真にアウトプットの完成と言えるもの）に仕上げるには、AIを活用した開発であっても数週間から数ヶ月のエンジニアリング作業を要する場合がある。AIは組織の非効率性（例：サイロ化）を浮き彫りにするため、チェンジエージェントの存在と変革への切迫感がこれまで以上に求められる。このギャップが暗黙のままでは、期待の衝突は避けられない。明確なアウトプット完成の定義を設け、プロダクトオーナーとプロダクト開発者が早期にコラボレーションすることで、ギャップを顕在化させるべきである。スクラムチームがスプリント（または1ヶ月）以内に価値をデリバリーできないのであれば、AIでは解決できない、より根本的な問題が存在している可能性がある。（SGEP/SoftwareEngineeringPractices、SGEP/ProductThinking、SGEP/ScrumExpanded）

<!-- ### The Continued Importance of Empirical Process Control -->

### 経験的プロセス制御の継続的な重要性 {#the-continued-importance-of-empirical-process-control}

<!-- If Scrum's pillars of transparency, inspection, and adaptation were important before, they are doubly so in the age of AI. AI can generate a flood of output and data that the Scrum Team can drown in or be misled by. It's crucial to make AI activities and results highly visible – for instance, clearly flagging AI-generated work items, sharing the rationale behind AI-driven decisions, and exposing any assumptions the AI made. This transparency enables effective inspection: the Sprint Review might be expanded to not only show what the Scrum Team built, but also how it was built with AI and whether any issues or learnings emerged. By inspecting both the product and the process, the team can catch problems early (e.g., the AI introduced a subtle UX inconsistency, or the team spent too long debugging an AI-written section). With those insights, adaptation follows. Scrum's framework of short Sprints and Sprint Retrospectives is an effective mechanism for iterating on how the Scrum Team uses AI. They can tweak their approach – perhaps adjusting the granularity of tasks given to the AI – and then observe the results in the next Sprint. The key is to treat AI integration as an empirical endeavor: formulate hypotheses about how to use AI effectively, test them on a small scale, review the outcomes, and adapt. Organizations that embrace empirical process control will be able to harness AI to its fullest advantage, steering its power to serve team and customer needs through integrated value streams. Those who abandon an empirical approach (for example, blindly trusting AI outputs or, conversely, dismissing AI after a single failure without learning) risk costly mistakes or missed opportunities. In the end, the heart of Scrum – learning fast and adjusting – is exactly what is needed to thrive in the fast-moving AI era. A continuous adaptive strategy is also required (see the separate strategy document). -->

スクラムの柱である透明性・検査・適応がこれまでも重要だったが、AI時代にはその重要性は倍増する。AIは膨大なアウトプットとデータを生み出すことができ、スクラムチームがその洪水に溺れたり、判断を誤ったりしかねない。AIの活動とその結果を高い透明性のもとで可視化することが不可欠である — たとえば、AIが生成した作業アイテムを明示的に識別し、AIに基づく意思決定の根拠を共有し、AIが置いた前提条件を開示する。この透明性が効果的な検査を可能にする：スプリントレビューでは、スクラムチームが何を構築したかだけでなく、AIをどのように活用して構築したか、そこからどのような問題や学びが生じたかも扱うことになるかもしれない。プロダクトとプロセスの両面を検査することで、問題の早期発見が可能になる（例：AIが微妙なUX上の不整合を持ち込んだ、あるいはAIが書いたセクションのデバッグに想定以上の時間を費やした）。こうした洞察を得ることで、適応へとつなげられる。スクラムにおける短いスプリントとスプリントレトロスペクティブの枠組みは、チームがAIの使い方を改善していくための効果的なメカニズムである。チームはアプローチを微調整し — たとえばAIに委ねるタスクの粒度を見直し — 次のスプリントでその効果を観察できる。鍵となるのは、AI統合を経験主義に基づく取り組みとして捉えることである：AIの効果的な使い方について仮説を立て、小規模にテストし、結果を検証して、適応する。経験的プロセス制御を実践する組織は、AIを最大限に活用し、統合されたバリューストリームを通じてその力をチームと顧客のニーズに役立てることができる。一方、経験主義のアプローチを捨てる者 — たとえばAIのアウトプットを盲信する、あるいは一度の失敗から学ぶことなくAIを見限る — は、重大なミスや機会損失を招くリスクがある。つまるところ、スクラムの本質　—　素早く学び、素早く適応すること　—　こそが、変化の激しいAI時代を勝ち抜くためにまさに求められるものである。継続的な適応戦略も不可欠である（別の戦略文書を参照）。

<!-- ## Part 3: Success Patterns of AI Integration -->

## パート3：良い状態とは - AI統合の成功パターン {#part-3-success-patterns-of-ai-integration}

<!-- **Organizations** that derive real value from AI share a few key traits [^20]. They treat AI integration as a system-wide capability, not a localized tool adoption—embedding it consistently from leadership to teams, and across the entire value stream, rather than isolating it within engineering or innovation units. These organizations maintain rigorous quality management—integrating AI-generated outputs only after proper peer review and testing, and using automated checks (including AI to assess AI's work) to enforce coding and delivery standards—while ensuring that faster AI-driven work does not fragment or interrupt the flow of value from idea to outcome. They scale validation in step with increased output, for example, by conducting user testing or collecting customer feedback immediately and frequently on AI-assisted changes. Human accountability remains explicit and non-negotiable: every AI-supported result is owned by a person or team, and decisions are never made blindly by AI. Culturally, these organizations promote transparency and learning—teams openly discuss where AI helps or hinders and adapt their ways of working accordingly. Most importantly, successful adopters remain outcome-focused. They measure success by impact on users and business results, not by volume of features delivered, and they are willing to discard AI-generated work that does not demonstrably create value. -->

AIから真の価値を引き出す**組織**には、いくつかの共通する特徴がある [^20]。AI統合を局所的なツール導入ではなく、システム全体のケイパビリティとして位置づけ、エンジニアリングやイノベーション部門に閉じ込めるのではなく、リーダーシップからチームまで、バリューストリーム全体に一貫して組み込んでいる。こうした組織は厳格な品質管理を維持し、AIが生成した出力を適切なピアレビューとテストを経てはじめて統合する。自動チェック（AIの成果物を評価するAIを含む）によってコーディングとデリバリーの基準を徹底しつつ、AIによる作業の高速化がアイデアからアウトカムへの価値の流れを分断しないようにしている。アウトプットの増加に合わせて検証もスケールさせ、たとえばAIが関与した変更に対して即座に、かつ頻繁にユーザーテストを実施したり顧客フィードバックを収集したりする。人間の説明責任は明示的かつ揺るがない原則である：AIが支援したすべての成果には必ず責任を負う個人またはチームが存在し、AIが独断で意思決定することはない。文化面では、透明性と学習を重視する — チームはAIがどこで役立ち、どこで妨げになるかをオープンに議論し、それに応じて働き方を見直す。最も重要なのは、AI統合に成功している組織はアウトカム志向を貫くことである。リリースした機能の量ではなく、ユーザーやビジネス成果への影響によって成功を測り、明確な価値を生まないAI生成の作業を躊躇なく破棄する。

<!-- Within **Scrum Teams**, effective patterns include using AI to tighten feedback loops (e.g., integrating feedback loops that evaluate each product change instantly) and to provide context-specific assistance (such as giving the AI access to the product's domain knowledge or past tickets so its suggestions are more relevant, a technique known as retrieval augmentation). Workflows are adapted so that AI handles well-defined, low-risk tasks, while humans concentrate on critical thinking, creative design, and final verification. High-performing teams also invest in retaining and growing human skills – they ensure Scrum Team members can still perform key tasks manually and understand the product domain deeply, so they can guide the AI and step in when needed. Some teams deliberately do occasional "manual days" to keep their proficiency sharp and to cross-check that AI outputs align with human understanding. -->

**スクラムチーム**内での効果的なパターンとしては、AIを活用してフィードバックループを強化すること（例：各プロダクト変更を即座に評価するフィードバックループの組み込み）や、文脈に応じた支援を得ること（例：プロダクトのドメイン知識や過去のチケットへのアクセスをAIに与え、提案の精度を高める — リトリーバル拡張生成（RAG）として知られる技法）が挙げられる。ワークフローは、明確に定義された低リスクのタスクをAIが担い、人間はクリティカルシンキング、創造的な設計、最終的な検証に集中する形に整えられる。ハイパフォーマンスのチームは、人間のスキルの保持と成長に投資する — スクラムチームメンバーが主要なタスクを自力で遂行でき、プロダクトドメインを深く理解している状態を保つことで、AIを適切に導き、必要な場面で介入できるようにしている。習熟度を維持し、AI出力が人間の理解と整合しているかを確認するために、あえて「ノーAIデー」を定期的に設けるチームもある。

<!-- For **Product Owners**, successful AI integration requires tightening—not loosening—the Definition of Output Done regarding quality, and the Definition of Outcome Done for business impact. As AI dramatically accelerates delivery, the Product Owner must ensure that faster output leads to faster learning with high quality, not just more features. High-performing Product Owners use AI-enabled speed to validate assumptions earlier and more frequently: they define clear outcome hypotheses, specify how success will be measured, and ensure that AI-assisted work is considered valuable only when it demonstrates real user or business impact. Product Backlog Items are grounded in explicit problems, acceptance criteria, and expected outcomes, providing clear direction for both humans and AI. The Definition of Outcome Done becomes the key steering mechanism: What evidence will show this change improved behavior, experience, or results? By insisting on measurable outcomes, rapid feedback, and a willingness to discard AI-generated output that fails to move the needle, Product Owners prevent teams from becoming AI-powered feature factories and instead turn increased delivery speed into sustained value creation. -->

**プロダクトオーナー**にとって、AI統合を成功させるには、品質に関するアウトプット完成の定義と、ビジネスインパクトに関するアウトカム完成の定義を緩めるのではなく、むしろ厳格にすることが求められる。AIがデリバリーを劇的に加速する中で、プロダクトオーナーはアウトプットの高速化が単なる機能の量産ではなく、高品質かつ迅速な学習につながるよう舵を取らなければならない。優れたプロダクトオーナーは、AIがもたらすスピードを活かして仮説をより早く、より頻繁に検証する：明確なアウトカム仮説を立て、成功の測定基準を定め、AI支援による作業が実際のユーザーインパクトやビジネスインパクトを示した場合にのみ価値があるとみなす。プロダクトバックログアイテムは、明示的な課題、受け入れ基準、期待されるアウトカムに根ざしており、人間にもAIにも明確な方向性を与える。アウトカム完成の定義が主要な舵取りの仕組みとなる：この変更が行動、体験、成果を改善したことを示すエビデンスは何か？測定可能なアウトカムの追求、迅速なフィードバック、成果に結びつかないAIによる生成物を躊躇なく捨てる姿勢を貫くことで、プロダクトオーナーはチームがAI駆動のフィーチャーファクトリーに陥ることを防ぎ、デリバリースピードの向上を持続的な価値創造へと転換する。

<!-- For **Product Developers**, successful AI integration depends on strengthening—not relaxing—the Definition of Output Done. High-performing teams ensure that every AI-assisted change meets the same quality bar as any human-written work: integrated, tested, reviewed, and demonstrably safe to release. AI is treated as a junior collaborator whose output is never accepted on trust; Product Developers remain fully accountable for the integrity of the Product Increment. Specification by Example plays a central role in making "Done" explicit: concrete, executable acceptance criteria and tests are defined before AI-assisted implementation begins, providing an unambiguous reference for both humans and AI. Continuous Integration, automated regression testing, and fast feedback loops operationalize the Definition of Done by answering the critical question, "How do we know we haven't broken anything else?" Essentially, this means (manually) creating a very tight test harness – of architectural compliance tests, Planguage for specification and Specification by Example tests guiding outcome, and more \- which has to be complied with by AI always (Generative AI has to hallucinate as it creates more out of less, it has to fill the gaps [^21]). In this way, the Definition of Output Done becomes the primary safety mechanism that allows AI to accelerate development while preserving quality, maintainability, and confidence in the Increment. -->

**プロダクト開発者**にとって、AI統合の成功は、アウトプット完成の定義を緩めるのではなく、むしろ強化することにかかっている。ハイパフォーマンスチームは、AIが支援した変更であっても人間が書いた成果物と同じ品質水準を満たすことを徹底する：統合済み、テスト済み、レビュー済みであり、リリースしても安全であることが実証されている。AIは、そのアウトプットを無条件に受け入れてはならないジュニアコラボレーターとして位置づけられる。プロダクトインクリメントの整合性に対する完全な説明責任は、引き続きプロダクト開発者が負う。実例による仕様（Specification by Example：SbE）は「完成」を明確にする上で中核的な役割を担う：具体的かつ実行可能な受け入れ基準とテストをAI支援の実装に先立って定義し、人間にもAIにも曖昧さのない判断基準を提供する。継続的インテグレーション、自動リグレッションテスト、迅速なフィードバックループは、「他の部分を壊していないとどうすれば分かるか？」という根本的な問いに答えることで、完成の定義を実務レベルで機能させる。具体的には、非常に厳密なテストハーネスを（手動で）構築することを意味する　—　アーキテクチャ準拠テスト、Planguage（品質要件を定量的に記述する計画言語）による仕様記述、実例による仕様（SbE）テストによるアウトカム（ふるまい）の検証など — これらにAIは常に適合しなければならない（生成AIは少ない情報からより多くを生み出す以上、必然的にギャップを補完する形で出力するためである [^21]）。こうして、アウトプット完成の定義は、品質・保守性・インクリメントへの信頼を守りながらAIによる開発の加速を可能にする、最も重要な安全メカニズムとなる。

<!-- ## Part 4: Practical Guidance for Implementation -->

## パート4：何をすべきか - 実装のための実践的ガイダンス {#part-4-practical-guidance-for-implementation}

<!-- **Lay the Groundwork:** Begin by establishing the conditions for safe and effective AI use. Set clear goals for why you are adopting AI (e.g., to reduce defect rates, to accelerate delivery of specific outcomes, to improve customer support response times) and ensure these goals are understood by all stakeholders. Develop basic guardrails: for example, update your Definition of Output Done to include "AI outputs must be reviewed and tested," and decide on initial acceptable use cases for AI. You might allow AI-generated code for non-critical components or testing, but not for high-risk modules until trust is built. Establish baseline metrics (e.g., current throughput, elapsed time, defect density, customer satisfaction scores) to objectively gauge AI's impact. Importantly, invest in team training and experimentation up front. Let team members play with the AI tools in a sandbox, perhaps run an internal hackathon to explore how AI could be used. The more comfortable and knowledgeable the team is, the smoother the integration will go. -->

**基盤を整える：** まず、安全かつ効果的にAIを活用するための土台づくりから始める。AIを採用する目的を明確にし（例：欠陥率の低減、特定のアウトカムのデリバリーの加速、カスタマーサポートの応答時間の短縮）、その目的をすべてのステークホルダーが共通理解していることを確認する。基本的なガードレールを設ける：たとえば、アウトプット完成の定義に「AI出力はレビューおよびテスト済みであること」を追加し、AIの初期ユースケースとして許容する範囲を定める。信頼が醸成されるまでは、非クリティカルなコンポーネントやテストにはAI生成コードを認めるが、高リスクモジュールには適用しないといった判断もあり得る。AIの影響を客観的に把握するためのベースライン指標（例：現在のスループット、経過時間、欠陥密度、顧客満足度スコア）を定めておく。重要なのは、チームのトレーニングと実験に先行投資することである。チームメンバーにサンドボックス環境でAIツールを自由に試させ、AIの活用方法を探る社内ハッカソンを開催するのもよい。チームの理解と習熟が深まるほど、統合はスムーズに進む。

<!-- **Begin with small, contained experiments:** But do not treat AI adoption as a point solution. Even when starting with a single team or use case, explicitly trace the entire value stream—from idea and discovery through development, release, and learning. Map where work is handed over between roles, teams, or systems, and where information changes form (for example, from conversation to document, document to ticket, ticket to code, code to report). These handovers and media breaks are where delay, loss of intent, and quality degradation most often occur. Use AI and agentic AI selectively to reduce friction at these points—such as summarizing intent across artifacts, keeping context intact across tools, automating low-risk transitions, or continuously checking alignment between requirements, implementation, and outcomes. At the same time, deliberately keep humans in the loop at every decision boundary. AI may assist, prepare, or recommend, but humans retain authority over prioritization, acceptance, and release decisions. The goal is not maximum automation, but a more integrated, faster flow of value with clear accountability. Starting small while optimizing across the full value stream ensures that early AI gains compound rather than creating new local optimizations or hidden bottlenecks. -->

**小規模で限定的な実験から始める：** ただし、AI導入を個別の課題解決策として扱ってはならない。単一のチームやユースケースから着手する場合でも、バリューストリーム全体を意識的にたどる — アイディエーション・ディスカバリーから開発、リリース、学習に至るまで。作業が役割・チーム・システム間で受け渡される箇所と、情報が形を変える箇所（たとえば、会話→ドキュメント、ドキュメント→チケット、チケット→コード、コード→レポート）を可視化する。こうした受け渡しやメディアの断絶こそ、遅延・意図の喪失・品質低下が最も起きやすい地点である。これらの地点での摩擦を減らすために、AIやエージェント型AIを選択的に活用する — たとえば、アーティファクト間で意図を要約する、ツール間でコンテキストを保持する、低リスクの移行を自動化する、要件・実装・アウトカム間の整合性を継続的に検証するなどである。同時に、あらゆる意思決定の境界で人間が関与する状態を意図的に維持する。AIは支援・準備・推奨を行うかもしれないが、優先順位付け・受け入れ・リリースの判断に対する最終権限は人間が持つ。目標は自動化の最大化ではなく、明確な説明責任のもとで、より統合的かつ迅速に価値が流れる状態をつくることである。バリューストリーム全体の最適化を視野に入れながら小さく始めることで、初期のAIによる成果が局所的な最適化や新たなボトルネックを生むのではなく、累積的な効果を発揮するようになる。

<!-- **Scale Up What Works:** Once initial kinks are worked out, gradually roll out AI practices to more teams and processes, focusing on the areas where the pilot demonstrated value. Share the pilot team's learnings through brown-bag sessions or ensemble work so that other teams can avoid pitfalls. Be prepared to invest in better tooling or infrastructure if needed – for example, connecting AI tools to your internal code repositories or knowledge bases to provide more context (thereby improving AI output relevance), or upgrading testing infrastructure to handle more frequent builds. Also, consider pairing less-experienced teams with "AI champions" or members of the pilot to mentor them. Meanwhile, update your measurement and feedback mechanisms organization-wide: if you're deploying faster with AI, ensure your user feedback loop (analytics, support feedback, etc.) is accelerated to validate the impact of changes quickly. Continue to monitor key indicators like quality metrics, cycle times, and customer satisfaction. Consider automated telemetry and monitoring alarms. If any of these start trending the wrong way at scale, be ready to pause and address the root cause (for example, if code duplication is rising, reinforce the refactoring policy or add an automated lint check). -->

**効果が実証されたものをスケールする：** 初期の試行錯誤がうまくいったら、パイロットで価値が確認された領域を中心に、AIプラクティスをより多くのチームやプロセスへ段階的に展開する。パイロットチームの学びはブラウンバッグセッション（ランチを利用したカジュアルな情報共有会や勉強会）やアンサンブルワーク（チーム一体での協働）を通じて共有し、他のチームが同じ落とし穴にはまらないようにする。必要に応じて、ツールやインフラへの追加投資も検討する — たとえば、AIツールを社内コードリポジトリや知識ベースに接続してコンテキストを充実させる（これによりAI出力の適合度が向上する）、あるいはビルド頻度の増加に対応できるようテストインフラを増強するなどである。経験の浅いチームには「AIチャンピオン」やパイロット経験者をメンターとして配置することも有効である。並行して、組織全体の測定・フィードバックの仕組みも見直す：AIによってデプロイが加速しているなら、変更の影響を迅速に検証できるようユーザーフィードバックループ（アナリティクス、サポート部門からのフィードバックなど）も同様に高速化する。品質指標、サイクルタイム、顧客満足度といった主要指標のモニタリングを継続する。自動テレメトリや監視アラートの導入も検討する。いずれかの指標がスケール拡大に伴い悪化傾向を示し始めた場合は、立ち止まって根本原因に対処する（たとえば、コード重複が増加しているならリファクタリング方針を強化するか、自動リントチェックを追加する）。

<!-- **Continuously Adapt:** AI technology will continue to evolve quickly, so build a capacity for continuous adaptation. Regularly review your AI usage norms. What worked last year might need revision as new models or features become available. Encourage teams to keep experimenting in small ways each Sprint – perhaps trying an AI tool for a new kind of task – and share their findings. Maintain open communication channels (e.g., an internal forum or chat group) where team members can share observations or tips on working with AI. If a new, more powerful model is released, have a plan to evaluate it (e.g., have one team pilot it for a Sprint and report back). Likewise, stay alert to new risks (e.g., if AI starts generating more persuasive but incorrect outputs, consider implementing an additional step, such as prompt clarification or verification). Keep the organization's governance adaptable; for example, your security or compliance review processes may need to evolve to address AI-generated content. By using Scrum's inspect-and-adapt cycle at the organizational level or organizational Plan-Do-Study-Act, you ensure that your AI integration doesn't stagnate. Above all, remain empirical: use data and observation to decide whether AI is helping and how to adjust. Maybe AI allows you to release twice as often – does customer value actually increase, or do you just end up releasing half-baked features? Watch those outcomes and adjust strategy accordingly. -->

**継続的に適応する：** AI技術は今後も急速に進化し続けるため、継続的に適応できる体制を築く。AI活用に関する規範や取り決めを定期的に見直す。昨年有効だったやり方も、新しいモデルや機能の登場に伴い改訂が必要になるかもしれない。各スプリントでチームが小さな実験を続けるよう促す — たとえば、新たな種類のタスクにAIツールを試してみるなど—そして、その結果をチーム間で共有する。AIとの協働に関する気づきやコツを交換できるオープンなコミュニケーションチャネル（社内フォーラムやチャットグループなど）を維持する。より強力な新しいモデルがリリースされた際は、評価のための計画を用意しておく（たとえば、1チームが1スプリントで試用し、結果を報告する）。同様に、新たなリスクにも注意を払う（たとえば、AIがもっともらしいが誤ったアウトプットを生成するようになった場合、プロンプトの明確化や検証といった追加ステップの導入を検討する）。組織のガバナンスを柔軟に保つことも重要である。たとえば、セキュリティやコンプライアンスのレビュープロセスは、AI生成コンテンツへの対応に合わせて進化させる必要があるかもしれない。組織レベルでスクラムの検査と適応サイクル、あるいは組織的なPDSA（Plan-Do-Study-Act）を実践することで、AI統合が停滞しないようにする。何より重要なのは、経験主義を貫くことである：AIが成果を生んでいるか、どう調整すべきかの判断には、データと観察を活用する。AIによってリリース頻度が2倍になったとして — 顧客価値は本当に向上しているのか、それとも中途半端な機能を量産しているだけなのか？ アウトカムを注視し、それに基づいて戦略を調整する。

<!-- **Common Pitfalls to Avoid:** Be mindful of classic mistakes. Do not assume AI can replace skilled people – it is a complement that still requires human guidance and oversight at every step. Avoid trying to do too much too soon; it's better to have a controlled rollout with feedback than a big splash that overwhelms your processes. Don't let the team sacrifice quality or skip testing in the rush to capitalize on AI speed – technical debt accumulated now will almost certainly nullify future gains. Also, guard against vanity metrics: an AI that doubles your team's velocity is counterproductive if the additional output is low value or piles up in unreleased backlogs. It's crucial to maintain focus on the true Definition of Output Done (working software that works) and the Definition of Outcome Done (delivers value). Culturally, don't punish experiments that fail – some AI uses will not pan out, and that's part of the learning curve. If team members fear blame, they will play it safe, and you'll never discover AI's potential. Finally, don't get caught in "analysis paralysis" or endless tool comparisons – pick a viable tool, start small, and learn by doing. The worst mistake in this fast-moving area is to do nothing. -->

**避けるべき典型的な落とし穴：** よくある失敗パターンに注意する。AIが熟練した人材の代替になると思い込んではならない — AIはあくまで補完的な存在であり、あらゆる段階で人間による指導と監督を必要とする。一度に多くを取り入れようとしない。プロセスを圧倒するような大規模な適用よりも、フィードバックを伴う段階的な導入の方が望ましい。AIのスピードを手にした勢いで品質の妥協やテストの省略を許してはならない — そうして蓄積された技術的負債は、将来の利益をほぼ確実に帳消しにする。見栄えのよい指標にも警戒する：チームのベロシティを倍増させるAIでも、追加されたアウトプットが低価値であったりリリースされないバックログに滞留したりするなら、むしろ逆効果である。真のアウトプット完成の定義（動くソフトウェアが実際に機能すること）とアウトカム完成の定義（価値を届けること）へのフォーカスを怠らないことが重要である。文化面では、失敗に終わった実験を罰しないこと — AI活用の試みがすべて成功するわけではなく、それは学びの過程の一部である。非難を恐れるチームメンバーは無難な選択しかしなくなり、AIの真の可能性は見出せない。最後に、「分析麻痺」や終わりのないツール比較に陥らないこと — まず使えるツールを選び、小さく始め、実践を通じて学ぶ。この急速に動く領域における最大の失敗は、何もしないことである。

<!-- ## Conclusion -->

## 結論 {#conclusion}

<!-- **AI is poised to dramatically reshape how software is developed – and, with it, the fortunes of companies that rely on digital products.** Those that successfully integrate AI into Scrum – maintaining a balance of speed and quality, automation and human judgment, output and outcome – stand to leap ahead in productivity and responsiveness to customer needs. Those who fail to adapt may quickly find themselves left behind in a world of exponential technological improvement. The following year or two likely represents a critical window of opportunity to build the capabilities and culture needed for an AI-driven future [^3]. -->

**AIはソフトウェアの開発のあり方を根底から変えようとしている—そしてそれに伴い、デジタルプロダクトに依存する企業の命運も左右される。** スクラムにAIをうまく統合できる組織 — スピードと品質、自動化と人間の判断、アウトプットとアウトカムのバランスを保ちながら—は、生産性と顧客ニーズへの対応力において大きく飛躍する位置にある。適応に失敗すれば、指数関数的に技術が進歩する世界の中で急速に取り残されかねない。今後1〜2年は、AI駆動の未来に必要な能力と文化を築くための極めて重要な機会であろう [^3]。

<!-- **The evidence suggests that the true differentiator is not who has the most sophisticated AI algorithms, but who can use AI most effectively, integratively, and strategically.** Scrum provides the framework for doing exactly that, but it requires recommitting to Scrum's essence at a new level. It means doubling down on clear goals, rapid feedback, and empowered teams – even as AI accelerates the pace. In this environment, the whole Scrum Team, especially the Product Owner's role as the navigator – deciding which problems to solve and ensuring the solutions deliver value – is more critical than ever. If AI is a supercharged engine of a ship, the Product Owner offers or co-creates the direction of travel, and the Product Developers run the ship. Organizations must invest in this product management capacity [^6] or risk building a lot of software that misses the mark, only faster. -->

**エビデンスが示唆するのは、真の差別化要因は最も洗練されたAIアルゴリズムを持つ者ではなく、AIを最も効果的かつ統合的・戦略的に活用できる者だということである。** スクラムはまさにそのためのフレームワークを提供するが、新たな次元でスクラムの本質に立ち返ることが求められる。すなわち、AIがペースを加速させる中にあっても、明確な目標、迅速なフィードバック、自律的なチームへの注力をいっそう強めることである。この環境では、スクラムチーム全体、とりわけナビゲーターとしてのプロダクトオーナーの役割—どの問題を解決すべきかを見極め、ソリューションが確実に価値を届けるようにする—がこれまで以上に重要になる。AIが船の強力なエンジンだとすれば、プロダクトオーナーは航路を示し、あるいは共に描き、プロダクト開発者が船を動かす。組織はこのプロダクトマネジメント能力に投資しなければならない [^6]。さもなければ、的外れなソフトウェアをより速く量産するだけに終わるリスクがある。

<!-- **In conclusion, integrating AI into Scrum is not a one-time effort but an ongoing process of experimentation and learning.** The technology will keep changing; what must remain constant is a commitment to empiricism, agility, and human-centric thinking. Scrum teams that internalize this will harness AI to achieve outcomes that were previously unimaginable, turning the AI revolution from a threat into a transformative opportunity. The time to start is now — the habits and ways of working that got you this far will also help you thrive with AI, as long as you're willing to keep adapting and growing. -->

**結論として、AIとスクラムの統合は一度きりの取り組みではなく、実験と学習を繰り返す継続的なプロセスである。** 技術は変わり続ける。変わらずに持ち続けるべきは、経験主義、アジリティ、そして人間中心の思考への揺るぎないコミットメントである。これを自らのものとしたスクラムチームは、AIを活用してかつては想像もできなかったアウトカムを実現し、AI革命を脅威から変革の好機へと転じるだろう。始めるべき時は今である—これまでの歩みを支えてきた習慣と働き方は、適応し成長し続ける意思さえあれば、AIとともに力を発揮する土台にもなる。

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
| AI-laggard | AI後発 | AI導入が遅れている組織 |
| Automation Bias | 自動化バイアス | 自動化システムを過度に信頼する傾向 |
| Cognitive Orchestrator | 認知オーケストレーター（司令塔） | AIの意図と制約を設定し、アウトカムを調整する役割 |
| Feature Factory | フィーチャーファクトリー | 価値検証なしに機能を大量生産する状態 |
| Generative AI Paradox | 生成AIパラドックス | AI導入率は高いがビジネスインパクトが低い現象 |
| Human-in-the-Loop | ヒューマン・イン・ザ・ループ | AI使用時に人間が監視・意思決定を維持する姿勢 |
| Retrieval Augmentation | リトリーバル拡張 | AIに企業固有の知識を提供して出力の関連性を向上させる技法 |
| Specification by Example (SbE) | 実例による仕様 | 具体例を使って要件を明確化するプラクティス |
| Vibe Code | バイブコード | プロトタイプを素早く作成するカジュアルなコーディング |
