---
# title: Psychological Safety in Scrum Teams (Expansion of the SGEP)
title: スクラムチームにおける心理的安全性（SGEP拡張版）
# subtitle: An empirical lens on safety as a foundation for learning and high performance in Scrum Teams
subtitle: スクラムチームにおける学習とハイパフォーマンスの基盤としての安全性に対する経験的視点
# description: A research-based examination of psychological safety in Scrum Teams, showing how fear undermines empiricism and how deliberate practices strengthen learning, transparency, and sustained high performance.
description: スクラムチームにおける心理的安全性の研究に基づく検討。恐れがどのように経験主義を損なうか、そして意図的なプラクティスがどのように学習、透明性、持続的なハイパフォーマンスを強化するかを示す。
# keywords:
# - Psychological safety
# - Scrum Teams
# - Empiricism
# - Transparency
# - Inspection and adaptation
# - Sprint Retrospective
# - Speaking up
# - Team learning
# - High performance
keywords:
  - 心理的安全性
  - スクラムチーム
  - 経験主義
  - 透明性
  - 検査と適応
  - スプリントレトロスペクティブ
  - 発言する
  - チーム学習
  - ハイパフォーマンス
author:
  - Joanna Płaskonka
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
  - /ja/psychological-safety-in-scrum-teams/2026.1/
---

<!-- ***Collected Resources for Scrum Guide Expansion Pack*** -->

**_スクラムガイド拡張パック 収録資料集_**

<!-- *This document is a collection of independent works. Each section retains its original license or copyright status, as indicated. Please refer to each section for specific usage rights and requirements.* -->

_この文書は独立した著作物のコレクションである。各セクションは示されているとおり、元のライセンスまたは著作権の状態を保持している。具体的な使用権と要件については、各セクションを参照してほしい。_

<!-- License/Copyright: [CC BY-NC-ND 4.0](https://creativecommons.org/licenses/by-nc-nd/4.0/) -->

ライセンス/著作権: [CC BY-NC-ND 4.0](https://creativecommons.org/licenses/by-nc-nd/4.0/)

<!-- Note: This section is included in its original, unaltered form with permission under the terms of the [CC BY-NC-ND 4.0](https://creativecommons.org/licenses/by-nc-nd/4.0/) license. No changes have been made. -->

注: このセクションは、[CC BY-NC-ND 4.0](https://creativecommons.org/licenses/by-nc-nd/4.0/) ライセンスの条項に基づき、許可を得て元の形式のまま収録されている。変更は加えられていない。

---

<!-- Scrum thrives when people are willing to share what they see, even when it is incomplete, inconvenient, or uncomfortable. Speaking up should be the default, not the exception. Psychological safety creates an environment for meaningful inspection and adaptation, which is how Scrum delivers learning and enables high performance. -->

スクラムは、人々が見ているものを、それが不完全、不都合、または不快であっても共有する意思があるときに繁栄する。発言することは例外ではなく、デフォルトであるべきである。心理的安全性は、意味のある検査と適応のための環境を作り出し、それがスクラムが学習を提供し、ハイパフォーマンスを可能にする方法である。

<!-- ### The fear tax in Scrum Teams -->

### スクラムチームにおける恐れの税金 {#the-fear-tax-in-scrum-teams}

<!-- Many Scrum practitioners have observed this: Scrum events that appear to work on the surface but feel empty. Sprint Retrospective that ends with safe, low-impact actions or none at all. No one challenges the goal, work, or assumptions during Sprint Planning, and silence replaces candid disagreement. You might also recognize this in the avoidance of hard questions and crucial conversations. Or in moments where status overrides expertise: a less senior product developer notices a quality risk, but the discussion is dominated by a more senior voice. These are often treated as facilitation or communications issues, but they are early signs of something deeper. -->

多くのスクラム実践者がこれを観察している：表面上は機能しているように見えるが、空虚に感じるスクラムイベント。安全で影響の少ないアクション、またはまったくアクションなしで終わるスプリントレトロスペクティブ。スプリントプランニング中に誰もゴール、作業、または前提に異議を唱えず、沈黙が率直な意見の不一致に取って代わる。難しい質問や重要な会話の回避にもこれを認識できるかもしれない。または、地位が専門知識を覆す瞬間：ジュニアのプロダクト開発者が品質リスクに気づくが、議論はよりシニアの声に支配される。これらはしばしばファシリテーションやコミュニケーションの問題として扱われるが、より深いものの初期兆候である。

<!-- This is common. It is not an exception. Scrum Teams pay a fear tax every Sprint. This cost is invisible at first glance, but it accumulates over time. The fear tax is driven by concerns about blame, embarrassment, appearing incompetent, or losing status or popularity. Fear consumes people's capacity even before the work starts. It shows up in small, everyday choices people make to self-protect: withholding concerns, softening language, delaying bad news, avoiding certain topics, or not asking for help. Each choice seems harmless, and it often feels like the best decision in that moment. Together, those choices create a compounding effect that degrades learning and decreases performance, even though no single moment looks dramatic. Fear delays risk detection and course correction. Problems do not disappear; they move downstream. Ultimately, the fear tax is often borne by the customer. -->

これは一般的である。例外ではない。スクラムチームは毎スプリント恐れの税金を払っている。このコストは一見見えないが、時間とともに蓄積される。恐れの税金は、非難、恥ずかしさ、無能に見えること、または地位や人気を失うことへの懸念によって駆動される。恐れは作業が始まる前でさえ人々の能力を消費する。それは人々が自己防衛するために行う小さな日常の選択に現れる：懸念を差し控える、言葉を和らげる、悪いニュースを遅らせる、特定のトピックを避ける、または助けを求めない。各選択は無害に見え、その瞬間には最良の決定のように感じられることが多い。それらの選択が一緒になると、単一の瞬間が劇的に見えなくても、学習を劣化させパフォーマンスを低下させる複合効果を生み出す。恐れはリスク検出と軌道修正を遅らせる。問題は消えない。下流に移動する。最終的に、恐れの税金はしばしば顧客が負担する。

<!-- Scrum is based on the pillars of transparency, inspection, and adaptation[^1]. When fear is present, transparency becomes selective, inspection narrows to carefully framed updates, and adaptation remains superficial. Fear constrains empiricism – the ability to learn from what is actually happening. -->

スクラムは透明性、検査、適応の柱に基づいている [^1]。恐れが存在するとき、透明性は選択的になり、検査は慎重に組み立てられた更新に狭まり、適応は表面的なままである。恐れは経験主義 - 実際に起こっていることから学ぶ能力 - を制約する。

<!-- Psychological safety (as defined by Amy Edmondson[^2]) is a capability Scrum Teams can develop and sustain to support learning and high performance. This work examines how psychological safety shows up in real Scrum work, how it affects learning and outcomes, and how Scrum Teams and leaders strengthen it through deliberate experiments in how they collaborate and learn from experience. For Scrum to be truly effective, it must create a safe space for learning. High performance emerges over time. -->

心理的安全性（Amy Edmondson [^2] の定義による）は、スクラムチームが学習とハイパフォーマンスをサポートするために開発し維持できる能力である。この著作は、心理的安全性が実際のスクラム作業でどのように現れるか、それが学習とアウトカムにどのように影響するか、そしてスクラムチームとリーダーがコラボレーションと経験からの学習の方法における意図的な実験を通じてそれをどのように強化するかを検討する。スクラムが真に効果的であるためには、学習のための安全な空間を作り出さなければならない。ハイパフォーマンスは時間とともに創発する。

<!-- ### What psychological safety is – and what it is not -->

### 心理的安全性とは何か - そして何ではないか {#what-psychological-safety-is-and-what-it-is-not}

<!-- According to Amy Edmondson, psychological safety is a shared belief that the team is safe for interpersonal risk-taking[^2]. An interpersonal risk is a risk someone takes when interacting with people. It means doing or saying something without knowing how others will react, for example, raising a hand in a meeting to admit you did not understand what was being discussed. Those reactions might range from supportive responses such as curiosity, attentive listening, and a willingness to help, to less supportive responses such as ignoring, blaming, or even assuming incompetence or questioning someone's credibility. Asking a question may be perceived as being uninformed or unprepared. Sharing a new idea may result in its dismissal or mockery rather than serious discussion. Admitting a mistake may lead to blame or shame, rather than to an invitation to explore why it happened. A team that is safe for interpersonal risk-taking is one in which people consistently feel that questions are welcome, ideas are thoughtfully considered, and mistakes are treated as opportunities to learn and improve, rather than as reasons for embarrassment, judgment, or punishment. -->

Amy Edmondsonによると、心理的安全性は、チームが対人リスクテイキングにとって安全であるという共有された信念である [^2]。対人リスクとは、人々と相互作用するときに誰かが取るリスクである。それは、他者がどのように反応するかを知らずに何かをしたり言ったりすることを意味する。例えば、議論されていることを理解していなかったことを認めるためにミーティングで手を挙げること。それらの反応は、好奇心、注意深い傾聴、助ける意志などの支持的な反応から、無視、非難、または無能を仮定したり誰かの信頼性を疑問視したりするなどのあまり支持的でない反応まで様々である。質問をすることは、情報がない、または準備ができていないと認識される可能性がある。新しいアイデアを共有することは、真剣な議論ではなく、却下や嘲笑につながる可能性がある。ミスを認めることは、なぜそれが起こったかを探る招待ではなく、非難や恥につながる可能性がある。対人リスクテイキングにとって安全なチームとは、人々が一貫して質問が歓迎され、アイデアが思慮深く検討され、ミスが恥ずかしさ、判断、または罰の理由ではなく、学習と改善の機会として扱われると感じるチームである。

<!-- The definition of psychological safety is empirical and research-based rather than aspirational. Psychological safety is not an individual trait. It is a team-level condition that forms over time through repeated experience of how others respond in different situations. It is not about comfort, niceness, or artificial harmony. When teams avoid disagreement or suppress difficult topics to preserve harmony, they prioritize comfort over psychological safety. Psychological safety enables constructive conflict, not its absence (see also Lencioni's model in [^3]). It is not a lack of accountability either. High psychological safety combined with high standards enables a learning and high-performance zone[^4]. In Scrum, high standards are expressed through clear expectations such as Definition of Output Done and Definition of Outcome Done, meaningful Sprint Goals, and accountability for outcomes. Google's Project Aristotle identified psychological safety as a key factor in team effectiveness[^5]. The learning zone is where Scrum Teams want to operate, because complex work requires learning. -->

心理的安全性の定義は、願望的ではなく経験的で研究に基づいている。心理的安全性は個人の特性ではない。それは、異なる状況で他者がどのように反応するかの繰り返しの経験を通じて時間とともに形成されるチームレベルの条件である。それは快適さ、優しさ、または人工的な調和についてではない。チームがハーモニーを維持するために不一致を避けたり困難なトピックを抑制したりするとき、彼らは心理的安全性よりも快適さを優先している。心理的安全性は建設的な対立を可能にするのであり、その不在ではない（[^3] のLencioniのモデルも参照）。それは説明責任の欠如でもない。高い心理的安全性と高い基準の組み合わせは、学習とハイパフォーマンスゾーンを可能にする [^4]。スクラムでは、高い基準はアウトプット完成の定義とアウトカム完成の定義、意味のあるスプリントゴール、アウトカムに対する説明責任などの明確な期待を通じて表現される。Googleのプロジェクト・アリストテレスは、心理的安全性をチームの効果性における主要な要因として特定した [^5]。学習ゾーンはスクラムチームが活動したい場所である。なぜなら、複雑な作業には学習が必要だからである。

<!-- Signs of psychological safety include: -->

心理的安全性の兆候には以下が含まれる：

<!-- - If I make a mistake, it will not be used against me. -->
<!-- - Speaking openly is expected. -->
<!-- - I can speak up, offer ideas, another point of view, and ask questions without fear of punishment or embarrassment. -->

- ミスをしても、それが私に不利に使われることはない。
- オープンに発言することが期待されている。
- 罰や恥ずかしさを恐れることなく、発言し、アイデアを提供し、別の視点を提供し、質問することができる。

<!-- These beliefs are situational; they can vary across situations and over time, even within the same Scrum Team. For example, the Scrum Team might feel safe during Sprint Retrospectives but not during Sprint Reviews. -->

これらの信念は状況的である。同じスクラムチーム内でも、状況や時間によって異なる可能性がある。例えば、スクラムチームはスプリントレトロスペクティブ中は安全だと感じるが、スプリントレビュー中はそうではないかもしれない。

<!-- Psychological safety is created and reinforced through how people interact. It develops through everyday interaction patterns. It is sensitive to how people treat one another in moments of uncertainty. Because it is shaped by experience rather than intention, psychological safety can shift quickly; a single dismissive comment or unresolved incident can have lasting effects on what people feel safe to say. Managers and stakeholders have disproportionate influence because their words, reactions, and decisions signal what is acceptable. When people fear that they will contradict, offend, or disappoint a leader, they may hold back questions or concerns, even when doing so harms the work. This is why leaders should speak last. The influence is not limited to formal roles. Team members also shape safety through their responses to ideas, mistakes, and disagreements. -->

心理的安全性は、人々がどのように相互作用するかを通じて作られ、強化される。それは日常の相互作用パターンを通じて発展する。それは不確実性の瞬間に人々がお互いをどのように扱うかに敏感である。心理的安全性は意図ではなく経験によって形成されるため、急速に変化する可能性がある。単一の軽蔑的なコメントや未解決のインシデントは、人々が何を言っても安全だと感じるかに持続的な影響を与える可能性がある。マネージャーとステークホルダーは不釣り合いな影響力を持っている。なぜなら、彼らの言葉、反応、決定が何が許容されるかを示すからである。人々がリーダーに反論、不快感を与える、または失望させることを恐れるとき、たとえそうすることが仕事に害を与えても、質問や懸念を控えるかもしれない。これがリーダーが最後に発言すべき理由である。影響力は公式の役割に限定されない。チームメンバーもアイデア、ミス、意見の不一致への反応を通じて安全性を形作る。

<!-- ### Psychological safety in the context of Scrum -->

### スクラムのコンテキストにおける心理的安全性 {#psychological-safety-in-the-context-of-scrum}

<!-- Voluntary interpersonal risk-taking is a needed core element of Scrum. It reflects openness, courage, and transparency in Scrum by design, because work and decisions are made visible and critiqued within the Scrum Team. People don't come to work to look ignorant, incompetent, or disruptive. Neither do they plan intentional errors. However, when people speak up, ask questions, or admit mistakes, they risk how others perceive them and interpret their intentions. A common response to reduce those risks is silence: don't speak, don't ask questions, don't challenge the status quo, don't offer ideas, and don't admit mistakes. Silence becomes a form of self-protection. This pattern, known as impression management[^6], leads to missed opportunities for learning, innovation, and product and organizational improvement. In Scrum Teams, impression management often entails concealing problems or doubts to appear competent, confident, and in control, rather than speaking candidly about what is actually happening. -->

自発的な対人リスクテイキングはスクラムの必要なコア要素である。それはスクラムにおける公開性、勇気、透明性を設計上反映している。なぜなら、作業と意思決定はスクラムチーム内で可視化され、批評されるからである。人々は無知、無能、または破壊的に見えるために仕事に来るわけではない。また、意図的なエラーを計画することもない。しかし、人々が発言し、質問し、またはミスを認めるとき、彼らは他者が彼らをどのように認識し、彼らの意図をどのように解釈するかのリスクを負う。それらのリスクを減らすための一般的な反応は沈黙である：発言しない、質問しない、現状に異議を唱えない、アイデアを提供しない、ミスを認めない。沈黙は自己防衛の一形態になる。印象管理 [^6] として知られるこのパターンは、学習、イノベーション、プロダクトと組織の改善の機会を逃すことにつながる。スクラムチームでは、印象管理はしばしば、実際に何が起こっているかについて率直に話すのではなく、有能で、自信があり、コントロールしているように見えるために問題や疑念を隠すことを伴う。

<!-- Scrum Teams often face interpersonal risks during formal events, informal meetings, or conversations. Those are the moments when Scrum Team members ask themselves, "Should I speak up or stay silent?" In Scrum, this internal dilemma shows up in concrete, specific situations: -->

スクラムチームは、公式イベント、非公式ミーティング、または会話中に対人リスクに直面することが多い。これらは、スクラムチームメンバーが自分自身に「発言すべきか、沈黙すべきか？」と問う瞬間である。スクラムでは、この内部のジレンマは具体的で特定の状況に現れる：

<!-- - **Reaction to Mistakes:** When a mistake or quality issue is noticed during the Daily Scrum, Sprint Retrospective, or Sprint Review, the team acknowledges it publicly. Instead of quietly fixing it in the background, they talk about it, understand it, and resolve it. More is the pity, as a focus on reducing errors leads to fewer insights[^7]. -->

- **ミスへの反応：** デイリースクラム、スプリントレトロスペクティブ、またはスプリントレビュー中にミスや品質問題が気づかれたとき、チームはそれを公に認める。バックグラウンドで静かに修正する代わりに、それについて話し、理解し、解決する。残念なことに、エラーを減らすことに焦点を当てると、インサイトが少なくなる [^7]。

<!-- - **Dealing with Issues:** When work becomes difficult during the Sprint, and impediments need to be surfaced early in the Daily Scrum rather than hidden to preserve the appearance of progress. -->

- **問題への対処：** スプリント中に作業が困難になり、進捗の外観を維持するために隠すのではなく、デイリースクラムで早期に障害を表面化させる必要があるとき。

<!-- - **Embracing Diversity:** When product assumptions, decisions, or technical approaches are challenged during Sprint Planning or Backlog Refinement, especially when that challenge comes from someone with less formal authority or seniority. -->

- **多様性を受け入れる：** スプリントプランニングまたはバックログリファインメント中にプロダクトの前提、決定、または技術的アプローチに異議が唱えられるとき、特にその異議がより低い公式の権限や年功序列を持つ誰かから来るとき。

<!-- - **Taking Risks:** When Scrum Teams are encouraged to run experiments, technical spikes, or discovery work where outcomes are uncertain, and learning may show up as "no, not this path" rather than visible success. -->

- **リスクを取る：** スクラムチームがアウトカムが不確実な実験、技術的スパイク、または発見作業を実行するよう奨励され、学習が可視的な成功ではなく「いいえ、この道ではない」として現れる可能性があるとき。

<!-- - **Asking for Help:** Asking for help, pairing, or clarification can expose gaps in understanding to peers or stakeholders. -->

- **助けを求める：** 助け、ペアリング、または明確化を求めることは、同僚やステークホルダーに理解のギャップを露出させる可能性がある。

<!-- - **Mutual Support:** When supporting a teammate under pressure means sharing responsibility for outcomes rather than protecting individual credibility (*mutual support*). -->

- **相互支援：** プレッシャー下のチームメイトをサポートすることが、個人の信頼性を保護するのではなく、アウトカムに対する責任を共有することを意味するとき（*相互支援*）。

<!-- - **Appreciation:** When contributing expertise or effort that improves long-term product quality or team effectiveness, knowing that this contribution may not be immediately visible or rewarded. -->

- **感謝：** 長期的なプロダクト品質やチームの効果性を向上させる専門知識や努力を貢献するとき、この貢献がすぐに可視的または報酬されない可能性があることを知っている。

<!-- These situations are not edge cases; they are everyday moments where psychological safety is either strengthened or diminished. The seven behavioral patterns named above are consistent with the Team Psychological Safety assessment vocabulary[^8]. -->

これらの状況はエッジケースではない。心理的安全性が強化されるか弱められるかの日常の瞬間である。上記の7つの行動パターンは、チーム心理的安全性評価の語彙 [^8] と一致している。

<!-- Scrum does not remove interpersonal risks. It makes them transparent. Psychological safety determines whether these moments become sources of learning and improved performance or reasons for self-protection. Because Scrum relies on frequent inspection, adaptation, and collective problem-solving, withholding effort directly limits Scrum's effectiveness. -->

スクラムは対人リスクを取り除かない。それらを透明にする。心理的安全性は、これらの瞬間が学習とパフォーマンス向上の源泉になるか、自己防衛の理由になるかを決定する。スクラムは頻繁な検査、適応、集団的な問題解決に依存しているため、努力を差し控えることはスクラムの効果性を直接制限する。

<!-- How teams respond to errors is a critical aspect of psychological safety in the context of Scrum. Product Developers are accountable for instilling quality by adhering to a Definition of Output Done[^9]. People make mistakes for different reasons, especially in complex work. Psychological safety does not mean tolerating repeated avoidable mistakes or reducing professionalism. Instead, it creates an environment in which team members feel safe being transparent about errors, the first step toward learning and improvement. Not all failures are the same, and responding to them requires judgment. Amy Edmondson defines 3 types of failures[^10]: -->

チームがエラーにどのように反応するかは、スクラムのコンテキストにおける心理的安全性の重要な側面である。プロダクト開発者は、アウトプット完成の定義を遵守することによって品質を植え付けることに説明責任を負う [^9]。人々は特に複雑な作業では、さまざまな理由でミスをする。心理的安全性は、繰り返し避けられるミスを許容したり、プロフェッショナリズムを減少させたりすることを意味しない。代わりに、チームメンバーがエラーについて透明であることを安全に感じる環境を作り出す。これは学習と改善への第一歩である。すべての失敗が同じではなく、それらに対応するには判断が必要である。Amy Edmondsonは3種類の失敗を定義している [^10]：

<!-- - **Basic failures:** Knowledge is well developed, and uncertainty is low. For example, misconfiguring a standard deployment pipeline or forgetting to follow a known test procedure. -->

- **基本的な失敗：** 知識は十分に開発されており、不確実性は低い。例えば、標準的なデプロイパイプラインの設定ミスや、既知のテスト手順に従うことを忘れる。

<!-- - **Complex failures:** Knowledge is well-developed, vulnerable to unexpected events, and uncertainty is moderate. For example, a production outage may be caused not by a single mistake but by a chain of smaller issues, or multiple teams may each make the most logical local decision, only to discover later that their choices conflict during integration. -->

- **複雑な失敗：** 知識は十分に開発されているが、予期しないイベントに脆弱であり、不確実性は中程度である。例えば、本番環境の停止は単一のミスではなく、より小さな問題の連鎖によって引き起こされる可能性がある。または、複数のチームがそれぞれ最も論理的なローカルの決定を行い、後になって統合中に彼らの選択が衝突することを発見する。

<!-- - **Intelligent failures:** Knowledge is limited, and uncertainty is high. For example, running a controlled experiment to validate a hypothesis that turns out to be wrong or attempting a novel technical approach that does not produce the expected performance. -->

- **知的な失敗：** 知識は限られており、不確実性は高い。例えば、間違っていることが判明する仮説を検証するための管理された実験を実行する、または期待されるパフォーマンスを生み出さない新しい技術的アプローチを試みる。

<!-- Psychological safety supports open discussion and learning from failures (or errors) that arise from uncertainty and exploration, whereas Scrum Teams openly discuss them and prevent the same avoidable mistakes from recurring. In that sense, the only true failure the Scrum Team faces is failing to learn and apply what was learned. The prime directive for Retrospectives is expressing one of the fundamental elements related to psychological safety – reaction to errors: "Regardless of what we discover, we understand and truly believe that everyone did the best job they could, given what they knew at the time, their skills and abilities, the resources available, and the situation at hand"[^11]. -->

心理的安全性は、不確実性と探索から生じる失敗（またはエラー）からのオープンな議論と学習をサポートする。一方、スクラムチームはそれらをオープンに議論し、同じ避けられるミスが再発することを防ぐ。その意味で、スクラムチームが直面する唯一の真の失敗は、学習し、学んだことを適用することに失敗することである。レトロスペクティブの最優先指令は、心理的安全性に関連する基本的な要素の1つ - エラーへの反応 - を表現している：「私たちが何を発見しようとも、私たちは全員が、その時点で知っていたこと、彼らのスキルと能力、利用可能なリソース、そして手元の状況を考慮して、できる限り最善の仕事をしたことを理解し、真に信じている」[^11]。

<!-- ### Scrum pillars, Scrum values, and psychological safety in practice -->

### スクラムの柱、スクラムの価値、そして実践における心理的安全性 {#scrum-pillars-scrum-values-and-psychological-safety-in-practice}

<!-- When discussing the connection between psychological safety and Scrum, a common question arises: do Scrum values create psychological safety, or does psychological safety enable Scrum values? Do Scrum pillars lead to safety, or does safety enable them? The more useful question is not which comes first (the chicken-or-egg dilemma), but how these elements reinforce or weaken one another over time. As Scrum is an empirical social system, it is worth examining how these conditions evolve through feedback loops created by Scrum events. This distinction matters because Scrum Teams often try to change behavior without examining how the system itself shapes it. -->

心理的安全性とスクラムの関係を議論するとき、一般的な質問が生じる：スクラムの価値は心理的安全性を作り出すのか、それとも心理的安全性がスクラムの価値を可能にするのか？スクラムの柱は安全性につながるのか、それとも安全性がそれらを可能にするのか？より有用な質問は、どちらが先か（鶏が先か卵が先かのジレンマ）ではなく、これらの要素が時間とともにどのように互いを強化または弱めるかである。スクラムは経験的な社会システムであるため、スクラムイベントによって作成されるフィードバックループを通じてこれらの条件がどのように進化するかを検討する価値がある。この区別は重要である。なぜなら、スクラムチームはしばしば、システム自体がどのように行動を形作るかを検討せずに行動を変えようとするからである。

<!-- The empirical Scrum pillars of transparency, inspection, and adaptation[^1] increase visibility and create opportunities for learning in Scrum Teams: -->

透明性、検査、適応という経験的なスクラムの柱 [^1] は、可視性を高め、スクラムチームに学習の機会を作り出す：

<!-- - Transparency exposes work, progress, assumptions, mistakes, and uncertainty. -->
<!-- - Inspection invites questioning, challenge, and evaluation. -->
<!-- - Adaptation requires acknowledging that previous decisions were incomplete or incorrect, not due to fault but to limited information and uncertainty. -->

- 透明性は作業、進捗、前提、ミス、不確実性を露出させる。
- 検査は質問、異議申し立て、評価を招く。
- 適応は、以前の決定が不完全または不正確であったことを認めることを必要とする。それは過失ではなく、限られた情報と不確実性のためである。

<!-- From that perspective, each Scrum pillar increases interpersonal risk. Speaking openly, admitting uncertainty, or challenging direction all happen publicly, in front of others. Thus, Scrum, by design, puts people in situations where social exposure is unavoidable. How teams respond to that exposure is where Scrum values come into play. -->

その観点から、各スクラムの柱は対人リスクを増加させる。オープンに発言すること、不確実性を認めること、または方向性に異議を唱えることは、すべて他者の前で公に行われる。したがって、スクラムは設計上、社会的露出が避けられない状況に人々を置く。チームがその露出にどのように反応するかが、スクラムの価値が作用する場所である。

<!-- Scrum as a framework does not create fear. Whenever people work closely with others, interpersonal risk is always present. Scrum reveals how teams respond to interpersonal risk and creates formal opportunities, through Scrum events, to reflect on and improve those responses. -->

フレームワークとしてのスクラムは恐れを作り出さない。人々が他者と密接に働くときはいつでも、対人リスクは常に存在する。スクラムはチームが対人リスクにどのように反応するかを明らかにし、スクラムイベントを通じて、それらの反応を振り返り改善するための公式の機会を作り出す。

<!-- The five Scrum values – commitment, focus, openness, respect, and courage – do not eliminate interpersonal risk-taking. They shape how Scrum Teams respond when it shows up[^12]: -->

5つのスクラムの価値 - 確約、集中、公開、尊敬、勇気 - は対人リスクテイキングを排除しない。それらは、それが現れたときにスクラムチームがどのように反応するかを形作る [^12]：

<!-- - **Openness** supports sharing incomplete or uncomfortable information. -->
<!-- - **Respect** reduces the social cost of speaking up and offering diverse perspectives, and curtails bluntness disguised as 'openness.' -->
<!-- - **Courage** supports challenge and dissent despite uncertainty. -->
<!-- - **Commitment** shifts attention from self-protection to a shared goal. -->
<!-- - **Focus** prevents noise and personal agendas from dominating the discussion. -->

- **公開** は不完全または不快な情報の共有をサポートする。
- **尊敬** は発言し多様な視点を提供することの社会的コストを減少させ、「公開」を装った無遠慮さを抑制する。
- **勇気** は不確実性にもかかわらず異議申し立てと反対意見をサポートする。
- **確約** は自己防衛から共有目標に注意を移す。
- **集中** はノイズや個人的なアジェンダが議論を支配することを防ぐ。

<!-- When these values are lived, interpersonal risk becomes manageable and creates opportunities for learning: what to improve, whether to pivot, and what to do next – about product decisions, quality, and ways of working. -->

これらの価値が実践されるとき、対人リスクは管理可能になり、学習の機会を作り出す：何を改善するか、ピボットすべきかどうか、次に何をすべきか - プロダクトの意思決定、品質、働き方について。

<!-- Psychological safety is not a value, a rule, or an intention. It is a belief that forms over time, based on what actually happens when people take interpersonal risks: when someone admits a mistake, when assumptions are challenged, and when bad news is delivered early. When the consequences are constructive, psychological safety increases. When the consequences are punitive, dismissive, or humiliating, psychological safety decreases, regardless of declared values. In this sense, psychological safety is an emergent property of how Scrum pillars and values are enacted in practice. Therefore, psychological safety becomes a functional requirement for Scrum to work as intended. -->

心理的安全性は価値、ルール、または意図ではない。それは、人々が対人リスクを取るときに実際に何が起こるかに基づいて、時間とともに形成される信念である：誰かがミスを認めるとき、前提に異議が唱えられるとき、悪いニュースが早期に伝えられるとき。結果が建設的であるとき、心理的安全性は増加する。結果が懲罰的、軽蔑的、または屈辱的であるとき、宣言された価値に関係なく、心理的安全性は減少する。この意味で、心理的安全性はスクラムの柱と価値が実践でどのように制定されるかの創発的特性である。したがって、心理的安全性はスクラムが意図したとおりに機能するための機能的要件になる。

<!-- Scrum pillars, values, and psychological safety co-evolve, forming a reinforcing loop: -->

スクラムの柱、価値、心理的安全性は共進化し、強化ループを形成する：

<!-- - Scrum pillars expose interpersonal risk. -->
<!-- - Scrum values shape responses to that risk. -->
<!-- - Those responses form psychological safety. -->
<!-- - Psychological safety determines whether transparency, inspection, and adaptation remain real. -->

- スクラムの柱は対人リスクを露出させる。
- スクラムの価値はそのリスクへの反応を形作る。
- それらの反応が心理的安全性を形成する。
- 心理的安全性は透明性、検査、適応が真実のままであるかどうかを決定する。

<!-- When this loop is reinforcing, Scrum supports sustained learning and enables high-performing Scrum Teams. When it is broken, Scrum degrades, and its benefits are diminished over time through everyday interactions and decisions. This is why psychological safety cannot be treated as a side concern. -->

このループが強化されているとき、スクラムは持続的な学習をサポートし、ハイパフォーマンスのスクラムチームを可能にする。それが壊れているとき、スクラムは劣化し、日常の相互作用と決定を通じて時間とともにその利益は減少する。これが心理的安全性を副次的な懸念として扱えない理由である。

<!-- ### Psychological safety as learning infrastructure in Scrum Teams -->

### スクラムチームにおける学習インフラストラクチャとしての心理的安全性 {#psychological-safety-as-learning-infrastructure-in-scrum-teams}

<!-- Scrum was designed to help people, teams, and organizations generate value through adaptive solutions for complex problem domains[^1]. It operates in conditions of uncertainty, where sustained performance depends on effective continuous learning and shared sense-making rather than perfect execution. Effective learning requires early exposure to uncertainty, incomplete understanding, weak signals, and emerging risks – before they lead to costly decisions made without sufficient insight. Psychological safety enables people to speak up before certainty exists – when learning still has the greatest leverage. When psychological safety supports speaking up, assumptions are challenged early, problems are surfaced while options remain open, and learning happens when change is still relatively inexpensive and course-correction opportunities remain available. Delayed understanding leads to late problem detection, fewer adaptation options, and the accumulation of hidden product, technical, and decision risks that remain out of sight. -->

スクラムは、人々、チーム、組織が複雑な問題ドメインに対する適応的なソリューションを通じて価値を生成することを支援するために設計された [^1]。それは不確実性の条件下で運営され、持続的なパフォーマンスは完璧な実行ではなく、効果的な継続的学習と共有されたセンスメイキングに依存する。効果的な学習は、十分なインサイトなしに行われるコストのかかる決定につながる前に、不確実性、不完全な理解、弱いシグナル、新興リスクへの早期の露出を必要とする。心理的安全性は、確実性が存在する前に - 学習がまだ最大のレバレッジを持っているときに - 人々が発言することを可能にする。心理的安全性が発言をサポートするとき、前提は早期に異議を唱えられ、オプションがまだ開いている間に問題が表面化し、変更がまだ比較的安価で軌道修正の機会がまだ利用可能なときに学習が起こる。理解の遅れは、問題検出の遅れ、適応オプションの減少、視界から隠れたままのプロダクト、技術、意思決定リスクの蓄積につながる。

<!-- High performance in Scrum emerges over time through accurate inspection, timely adaptation, and repeated learning cycles. Psychological safety is not an objective for Scrum Teams; it is an enabling condition for the learning that leads to high performance. In that sense, psychological safety functions as infrastructure for delivering high value in an effective way: it allows learning to be reliable and sustained over time, rather than episodic or accidental. Because psychological safety can be observed and assessed across multiple dimensions, Scrum Teams can see whether this infrastructure is strengthening or weakening. Like any form of infrastructure, it is rarely noticed when it works well, but when it diminishes, it limits what Scrum Teams can achieve. This infrastructure emerges and evolves through everyday interactions and decisions. -->

スクラムにおけるハイパフォーマンスは、正確な検査、タイムリーな適応、繰り返される学習サイクルを通じて時間とともに創発する。心理的安全性はスクラムチームの目標ではない。それはハイパフォーマンスにつながる学習のための有効化条件である。その意味で、心理的安全性は効果的な方法で高い価値を提供するためのインフラストラクチャとして機能する：それは学習が断続的または偶発的ではなく、信頼性があり時間とともに持続することを可能にする。心理的安全性は複数の次元にわたって観察および評価できるため、スクラムチームはこのインフラストラクチャが強化されているか弱化しているかを見ることができる。あらゆる形式のインフラストラクチャと同様に、それがうまく機能しているときはほとんど気づかれないが、それが減少するとき、スクラムチームが達成できることを制限する。このインフラストラクチャは日常の相互作用と決定を通じて創発し進化する。

<!-- ### How leadership signals shape psychological safety -->

### リーダーシップのシグナルが心理的安全性をどのように形作るか {#how-leadership-signals-shape-psychological-safety}

<!-- Psychological safety is shaped by what the system consistently signals as acceptable more than by what people say they value. In Scrum contexts, this system comprises decision-making structures, feedback loops, incentives, and interaction norms that enable how people raise concerns, challenge assumptions, or acknowledge uncertainty. For example, whether insights from the Sprint Retrospective lead to meaningful decisions and change, or whether missed Sprint Goals trigger reflection or blame. -->

心理的安全性は、人々が価値があると言うことよりも、システムが一貫して許容可能として示すものによって形作られる。スクラムのコンテキストでは、このシステムは意思決定構造、フィードバックループ、インセンティブ、および人々が懸念を提起し、前提に異議を唱え、または不確実性を認める方法を可能にする相互作用規範で構成される。例えば、スプリントレトロスペクティブからのインサイトが意味のある決定と変化につながるかどうか、または達成されなかったスプリントゴールが振り返りを引き起こすか非難を引き起こすか。

<!-- Managers and stakeholders have disproportionate influence because they control or strongly affect consequences such as approval, recognition, escalation, and how outcomes are interpreted – including what counts as success. How they respond in moments of uncertainty, error, or dissent sends a signal to everyone watching, including those who stay silent. When mistakes are met with curiosity and analysis, people learn they can speak up about them. When challenges are dismissed, ignored, or subtly penalized (such as being excluded from future discussions), people learn to withhold, even when no explicit blame is issued. Silence is often rational or emotional self-protection, not disengagement, because people are paying attention to the system's signals. This effect is amplified by status, hierarchy, seniority, and real or perceived expertise. In collective decision-making settings, lower-influence or less senior roles entail greater interpersonal risk when they question assumptions or raise concerns. If those contributions are consistently dismissed or minimized, expertise is suppressed, and learning degrades over time. -->

マネージャーとステークホルダーは不釣り合いな影響力を持っている。なぜなら、彼らは承認、認識、エスカレーション、およびアウトカムがどのように解釈されるか - 何が成功とみなされるかを含む - などの結果をコントロールするか強く影響するからである。不確実性、エラー、または反対意見の瞬間に彼らがどのように反応するかは、沈黙している人を含め、見ている全員にシグナルを送る。ミスが好奇心と分析で迎えられるとき、人々はそれについて発言できることを学ぶ。異議申し立てが却下、無視、または微妙に罰せられるとき（将来の議論から除外されるなど）、明示的な非難が発せられなくても、人々は差し控えることを学ぶ。沈黙はしばしば合理的または感情的な自己防衛であり、離脱ではない。なぜなら、人々はシステムのシグナルに注意を払っているからである。この効果は、地位、階層、年功序列、および実際のまたは認識された専門知識によって増幅される。集団的意思決定の設定では、影響力が低いまたはよりジュニアの役割は、前提に質問したり懸念を提起したりするときに、より大きな対人リスクを伴う。それらの貢献が一貫して却下または最小化される場合、専門知識は抑制され、学習は時間とともに劣化する。

<!-- Leadership influence is not limited to formal roles. Experienced Product Developers, Scrum Masters, and Product Owners act as informal leaders through facilitation choices, reactions to tensions, and responses to dissent. Non-intervention is also a signal – often the strongest one. When dismissive behaviour goes unaddressed, the system quietly teaches what is unsafe to say. -->

リーダーシップの影響力は公式の役割に限定されない。経験豊富なプロダクト開発者、スクラムマスター、プロダクトオーナーは、ファシリテーションの選択、緊張への反応、反対意見への対応を通じて非公式のリーダーとして行動する。非介入もシグナルである - しばしば最も強いものである。軽蔑的な行動が対処されないとき、システムは静かに何が言うのに安全でないかを教える。

<!-- Leaders can foster psychological safety, but their work is never done. It is sustained through continual practice. Building and reinforcing the work environment where people can learn, innovate, and grow is an ongoing work[^4]. Because psychological safety is shaped through everyday interactions, it can be strengthened through deliberate actions rather than cultural slogans. And it starts with small choices. -->

リーダーは心理的安全性を育むことができるが、彼らの仕事は決して終わらない。それは継続的な実践を通じて維持される。人々が学習し、革新し、成長できる職場環境を構築し強化することは継続的な仕事である [^4]。心理的安全性は日常の相互作用を通じて形作られるため、文化的なスローガンではなく意図的な行動を通じて強化できる。そしてそれは小さな選択から始まる。

<!-- ### Inspecting the conditions for learning -->

### 学習の条件を検査する {#inspecting-the-conditions-for-learning}

<!-- Scrum requires transparency to enable inspection and adaptation. If something is not visible, the Scrum Team cannot meaningfully change it. The same principle applies to psychological safety, and the whole team shares responsibility for inspecting it. When teams assume safety based on intent, values statements, or the absence of visible conflict, they lose the ability to inspect how their system actually behaves. -->

スクラムは検査と適応を可能にするために透明性を必要とする。何かが可視的でなければ、スクラムチームはそれを意味のある方法で変更できない。同じ原則が心理的安全性に適用され、チーム全体がそれを検査する責任を共有する。チームが意図、価値ステートメント、または可視的な対立の不在に基づいて安全性を仮定するとき、彼らはシステムが実際にどのように振る舞うかを検査する能力を失う。

<!-- Scrum events make team behavior visible. Who speaks up during Sprint Planning? What is raised – and what is avoided – in the Daily Scrum? Which assumptions are challenged in Sprint Review discussions? What is named, and what is softened, in the Sprint Retrospective? These are observable signals, not opinions. By treating psychological safety as an inspectable condition rather than a cultural label, Scrum Teams can examine where transparency leads to learning and where it breaks down. Silence, politeness, or quick alignment are not conclusions; they are data points. Interpreted through inspection, they reveal how the team responds to uncertainty, error, disagreement, and risk. -->

スクラムイベントはチームの行動を可視化する。スプリントプランニング中に誰が発言するか？デイリースクラムで何が提起され、何が避けられるか？スプリントレビューの議論でどの前提に異議が唱えられるか？スプリントレトロスペクティブで何が名付けられ、何が和らげられるか？これらは意見ではなく、観察可能なシグナルである。心理的安全性を文化的なラベルではなく検査可能な条件として扱うことで、スクラムチームは透明性がどこで学習につながり、どこで崩壊するかを検討できる。沈黙、礼儀正しさ、または迅速な整合は結論ではない。それらはデータポイントである。検査を通じて解釈されると、チームが不確実性、エラー、意見の不一致、リスクにどのように反応するかを明らかにする。

<!-- This shift – from assuming safety to inspecting its effects – allows teams to adapt deliberately rather than react implicitly. Psychological safety becomes part of empiricism: something shaped through repeated interactions and outcomes, not declared or assumed, just like product learning. -->

このシフト - 安全性を仮定することからその効果を検査することへ - により、チームは暗黙的に反応するのではなく、意図的に適応できる。心理的安全性は経験主義の一部になる：プロダクト学習と同様に、宣言または仮定されるのではなく、繰り返しの相互作用とアウトカムを通じて形作られるもの。

<!-- Psychological safety is not binary. It varies by situation and topic and manifests differently across interpersonal risks. A team may feel safe asking technical questions, yet unsafe challenging Product Backlog ordering, raising strategic risks, or delivering bad news. In such cases, people learn precisely where speaking up is costly and where silence is safer. We can examine psychological safety empirically and measure it, taking its elements into account (such as taking risk, asking for help, or dealing with issues), so Scrum Teams do not rely on intuition alone. Amy Edmondson developed the Psychological Safety Index (PSI)[^13]. Building on her research and his own[^14], Peter Cauwelier created the Team Psychological Safety for Team and the Team Psychological Safety for Leader assessments[^8]. These tools quantify psychological safety through measurable indicators and identify areas requiring attention and improvement, helping teams and leaders translate insights into concrete next steps. Viewing psychological safety as multidimensional enables Scrum Teams to identify which risks are perceived as unsafe and how this constrains learning, decision-making, and outcomes. -->

心理的安全性はバイナリではない。状況とトピックによって異なり、対人リスクによって異なる形で現れる。チームは技術的な質問をすることは安全だと感じるかもしれないが、プロダクトバックログの順序に異議を唱えること、戦略的リスクを提起すること、または悪いニュースを伝えることは安全でないと感じるかもしれない。そのような場合、人々は発言することがコストがかかる場所と沈黙がより安全な場所を正確に学ぶ。私たちは心理的安全性を経験的に検討し、その要素（リスクを取る、助けを求める、問題に対処するなど）を考慮に入れて測定できるため、スクラムチームは直感だけに頼らない。Amy Edmondsonは心理的安全性指数（PSI）を開発した [^13]。彼女の研究と彼自身の研究 [^14] に基づいて、Peter Cauweliersはチーム心理的安全性（Team）とチーム心理的安全性（Leader）の評価を作成した [^8]。これらのツールは測定可能な指標を通じて心理的安全性を定量化し、注意と改善が必要な領域を特定し、チームとリーダーがインサイトを具体的な次のステップに変換するのを支援する。心理的安全性を多次元的に見ることで、スクラムチームはどのリスクが安全でないと認識されているか、そしてこれが学習、意思決定、アウトカムをどのように制約するかを特定できる。

<!-- ### Strengthening psychological safety through deliberate learning practices -->

### 意図的な学習プラクティスを通じて心理的安全性を強化する {#strengthening-psychological-safety-through-deliberate-learning-practices}

<!-- Psychological safety does not improve through slogans, motivational pictures on the wall, one-off workshops, or encouragement alone. It is shaped through repeated practice – specifically, how Scrum Teams structure learning in everyday work and how they and their stakeholders respond to the outcomes of that learning. -->

心理的安全性はスローガン、壁のモチベーション画像、一回限りのワークショップ、または励ましだけでは改善しない。それは繰り返しのプラクティス - 具体的には、スクラムチームが日常の仕事で学習をどのように構造化し、彼らとステークホルダーがその学習のアウトカムにどのように反応するか - を通じて形作られる。

<!-- Key characteristics of such practices include: -->

そのようなプラクティスの主要な特徴には以下が含まれる：

<!-- - Structured inquiry instead of unstructured discussion. Practices that emphasize questions over statements reduce the interpersonal cost of participation (for instance, Action Learning[^15][^16]). When questioning is built into the format, speaking up becomes part of the process rather than a personal risk. -->

- 非構造化の議論ではなく構造化された探求。ステートメントよりも質問を強調するプラクティスは、参加の対人コストを減少させる（例えば、アクションラーニング [^15][^16]）。質問がフォーマットに組み込まれているとき、発言することは個人的なリスクではなくプロセスの一部になる。

<!-- - Regular, disciplined reflection. Sprint Reviews and Sprint Retrospectives that focus on understanding causes, extracting learning, and acting on insights, rather than assigning blame, reinforce the expectation that mistakes and difficulties are inputs for improvement. Scrum Teams can intentionally structure these conversations using facilitation approaches such as Liberating Structures[^17]. -->

- 定期的で規律ある振り返り。非難を割り当てるのではなく、原因の理解、学習の抽出、インサイトに基づく行動に焦点を当てるスプリントレビューとスプリントレトロスペクティブは、ミスと困難が改善のためのインプットであるという期待を強化する。スクラムチームはリベレイティングストラクチャーズ [^17] などのファシリテーションアプローチを使用してこれらの会話を意図的に構造化できる。

<!-- - Making learning visible. When Scrum Teams explicitly share what they learned (including negative or inconclusive outcomes), learning becomes a recognized form of progress. This reduces pressure to present certainty or success prematurely. -->

- 学習を可視化する。スクラムチームが学んだことを（否定的または結論の出ないアウトカムを含めて）明示的に共有するとき、学習は認識された形式の進歩になる。これは確実性や成功を時期尚早に提示するプレッシャーを減少させる。

<!-- - Normalizing intelligent failure while still aiming at high standards. Small, contained experiments with explicit learning intent clarify which failures are acceptable and why. This protects psychological safety while maintaining professional rigor. -->

- 高い基準を目指しながら知的な失敗を正常化する。明示的な学習意図を持つ小さく含まれた実験は、どの失敗が許容可能でなぜかを明確にする。これはプロフェッショナルな厳格さを維持しながら心理的安全性を保護する。

<!-- - Consistent responses to voice. How questions, challenges, and concerns are received matters more than how often they are invited. Consistency over time is what turns isolated safe moments into stable expectations. -->

- 発言への一貫した反応。質問、異議申し立て、懸念がどのように受け取られるかは、それらがどのくらい頻繁に招待されるかよりも重要である。時間の経過に伴う一貫性が、孤立した安全な瞬間を安定した期待に変えるものである。

<!-- - Scrum Teams may adopt a simple "red team" code word to invite time‑boxed, constructive dissent in events such as Sprint Reviews and Sprint Retrospectives, or "in the moment" (which can also be called "playing devil's advocate"). When invoked, Scrum Team members actively challenge assumptions and explore alternatives while staying respectful and outcome‑focused, which supports psychological safety by signalling that speaking up and questioning the status quo are legitimate and valued. Toxic positivity must be avoided. -->

- スクラムチームは、スプリントレビューやスプリントレトロスペクティブなどのイベント、または「その瞬間」（「悪魔の代弁者を演じる」とも呼ばれる）でタイムボックス化された建設的な反対意見を招くためのシンプルな「レッドチーム」コードワードを採用できる。それが呼び出されたとき、スクラムチームメンバーは敬意を払いアウトカムに焦点を当てながら、積極的に前提に異議を唱え代替案を探る。これは発言と現状への疑問が正当で価値があることを示すことで心理的安全性をサポートする。有害なポジティブさは避けなければならない。

<!-- Small everyday choices build or erode psychological safety: structured inquiry prevents dominant voices, disciplined reflection focuses on learning, not blame, and transparent experiments – whether successful or not – show that speaking up has an impact. These practices are strengthened when leaders model the behaviours that make learning safe and expected. Amy Edmondson proposes 3 leadership behaviors that support a psychological safety climate[^18]: -->

小さな日常の選択が心理的安全性を構築または侵食する：構造化された探求は支配的な声を防ぎ、規律ある振り返りは非難ではなく学習に焦点を当て、透明な実験 - 成功するかどうかにかかわらず - は発言することがインパクトを持つことを示す。リーダーが学習を安全で期待されるものにする行動をモデル化するとき、これらのプラクティスは強化される。Amy Edmondsonは心理的安全性の気候をサポートする3つのリーダーシップ行動を提案している [^18]：

<!-- - Frame the work as a learning problem. -->
<!-- - Acknowledge your own fallibility. -->
<!-- - Model curiosity. -->

- 作業を学習の問題として枠組みする。
- 自分自身の誤りやすさを認める。
- 好奇心をモデル化する。

<!-- A variety of additional leader practices and tools can complement these behaviours[^19]. -->

さまざまな追加のリーダープラクティスとツールがこれらの行動を補完できる [^19]。

<!-- Over time, these practices shift the Scrum Team's work climate toward one in which learning is expected and shared. Strengthening psychological safety helps Scrum Teams learn from experience, adapt deliberately, and improve performance over time. -->

時間の経過とともに、これらのプラクティスはスクラムチームの仕事の気候を、学習が期待され共有される気候へとシフトさせる。心理的安全性を強化することは、スクラムチームが経験から学び、意図的に適応し、時間とともにパフォーマンスを向上させるのを助ける。

<!-- ### Summary -->

### まとめ {#summary}

<!-- Scrum exposes uncertainty and invites learning, but effective learning only happens when people feel safe to take interpersonal risks. Psychological safety is a practical, inspectable condition shaped by how teams speak, decide, respond to errors, and challenge assumptions every day. When managers, stakeholders, and Scrum Teams reinforce behaviours that make voice safe, transparency becomes real, inspection becomes honest, and adaptation becomes meaningful. When they do not, Scrum devolves into empty mechanics and hidden risk. Strengthening psychological safety is therefore inseparable from improving empirical process control and achieving high performance in Scrum. -->

スクラムは不確実性を露出させ学習を招くが、効果的な学習は人々が対人リスクを取ることを安全だと感じるときにのみ起こる。心理的安全性は、チームが毎日どのように発言し、決定し、エラーに反応し、前提に異議を唱えるかによって形作られる実践的で検査可能な条件である。マネージャー、ステークホルダー、スクラムチームが発言を安全にする行動を強化するとき、透明性は現実になり、検査は正直になり、適応は意味のあるものになる。彼らがそうしないとき、スクラムは空虚な仕組みと隠されたリスクに変質する。したがって、心理的安全性を強化することは、経験的プロセス制御を改善し、スクラムでハイパフォーマンスを達成することと切り離せない。

<!-- ## References -->

## 参考文献 {#references}

[^1]: Scrum Guide 2020 (2020) *Scrum Guide*. Available at: [https://scrumguides.org/scrum-guide.html](https://scrumguides.org/scrum-guide.html) (Accessed: 7 January 2026).

[^2]: Edmondson, A. (1999) 'Psychological safety and learning behavior in work teams', *Administrative Science Quarterly*, 44(2), pp. 350–383.

[^4]: Edmondson, A.C. (2018) *The fearless organization: Creating psychological safety in the workplace for learning, innovation, and growth*. Hoboken, NJ: John Wiley & Sons.

[^5]: Google Re:Work (no date) *Understanding team effectiveness*. Available at: [https://rework.withgoogle.com/intl/en/guides/understanding-team-effectiveness](https://rework.withgoogle.com/intl/en/guides/understanding-team-effectiveness) (Accessed: 7 January 2026).

[^6]: Schlenker, B.R. (1980) *Impression management*. Monterey, CA: Brooks/Cole.

[^7]: Klein, G. (2017) *Seeing What Others Don't: The Remarkable Ways We Gain Insights*. London: John Murray Press.

[^8]: TeamAsOne (no date) *Psychological safety*. Available at: [https://teamasone.com/psychological-safety/](https://teamasone.com/psychological-safety/) (Accessed: 7 January 2026).

[^9]: Scrum Expansion (2025) *Scrum Guide Expansion Pack*. Available at: [https://scrumexpansion.org/scrum-guide-expansion-pack/](https://scrumexpansion.org/scrum-guide-expansion-pack/) (Accessed: 7 January 2026).

[^10]: Kerth, N.L. (2013) *Project retrospectives: A handbook for team reviews*. Boston, MA: Addison-Wesley.

[^12]: Verheyen, G. (no date) *The Scrum values*. Available at: [https://guntherverheyen.com/library/the-scrum-values/](https://guntherverheyen.com/library/the-scrum-values/) (Accessed: 7 January 2026).

[^13]: Fearless Organization Scan (no date) *Understanding the Psychological Safety Index (PSI)*. Available at: [https://fearlessorganizationscan.com/understanding-the-psychological-safety-index-psi](https://fearlessorganizationscan.com/understanding-the-psychological-safety-index-psi) (Accessed: 7 January 2026).

[^14]: Cauwelier, P. (2016) *The influence of team psychological safety on team knowledge creation: A comparative study between Thai, French and American engineering teams*. PhD thesis.

[^15]: World Institute for Action Learning (no date) *WIAL*. Available at: [https://wial.org/](https://wial.org/) (Accessed: 7 January 2026).

[^16]: Marquardt, M. (2011) *Optimizing the power of action learning: Real-time strategies for developing leaders, building teams and transforming organizations*. London: Nicholas Brealey.

[^17]: Liberating Structures (no date) *Liberating Structures*. Available at: [https://www.liberatingstructures.com/](https://www.liberatingstructures.com/) (Accessed: 7 January 2026).

[^18]: YouTube (2020) *Amy Edmondson: The Fearless Organization* [Video]. Available at: [https://www.youtube.com/watch?v=LhoLuui9gX8](https://www.youtube.com/watch?v=LhoLuui9gX8) (Accessed: 7 January 2026).

[^19]: Helbig, K. and Norman, M. (2023) *The Psychological Safety Playbook: Lead More Powerfully by Being More Human*. Vancouver: Page Two Press.

---

## 本文書の用語 {#glossary}

共通用語については [スクラムガイド拡張パック用語集](/ja/scrum-guide-expanded/2026.1/#スクラムガイド拡張パック用語集) を参照。

| 英語 | 日本語 | 説明 |
| --- | --- | --- |
| Psychological Safety | 心理的安全性 | チームが対人リスクテイキングにとって安全であるという共有された信念 |
| Fear Tax | 恐れの税金 | 恐れによってスクラムチームが毎スプリント払う見えないコスト |
| Interpersonal Risk | 対人リスク | 人々と相互作用するときに取るリスク（発言、質問、ミスの認知など） |
| Impression Management | 印象管理 | 他者からの認識を管理するために行動を調整するパターン |
| Learning Zone | 学習ゾーン | 高い心理的安全性と高い基準が組み合わさった状態 |
| Basic Failure | 基本的な失敗 | 知識が十分で不確実性が低い状況での失敗 |
| Complex Failure | 複雑な失敗 | 予期しないイベントに脆弱で中程度の不確実性がある状況での失敗 |
| Intelligent Failure | 知的な失敗 | 知識が限られ不確実性が高い状況での失敗（実験や探索から生じる） |
| Red Team | レッドチーム | タイムボックス化された建設的な反対意見を招くコードワード |
| Action Learning | アクションラーニング | 質問を通じて学習を促進する構造化されたプラクティス |
| Liberating Structures | リベレイティングストラクチャーズ | 全員の参加を促進するファシリテーション手法群 |
