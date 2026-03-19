---
# title: Psychological Safety in Scrum Teams (Expansion of the SGEP)
title: スクラムチームにおける心理的安全性（SGEP拡張版）
# subtitle: An empirical lens on safety as a foundation for learning and high performance in Scrum Teams
subtitle: スクラムチームにおける学習と高パフォーマンスの基盤となる安全性を経験主義の視点から考察する
# description: A research-based examination of psychological safety in Scrum Teams, showing how fear undermines empiricism and how deliberate practices strengthen learning, transparency, and sustained high performance.
description: スクラムチームにおける心理的安全性を研究に基づいて考察し、恐れがどのように経験主義を損なうか、そして意図的な実践がどのように学習、透明性、持続的な高パフォーマンスを強化するかを示す。
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
  - 発言
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

_本書は、独立した著作物を収録したものである。各セクションは記載の通り、オリジナルのライセンスや著作権状況を保持している。特定の使用権限と要件については、各セクションを参照して欲しい。_

<!-- License/Copyright: [CC BY-NC-ND 4.0](https://creativecommons.org/licenses/by-nc-nd/4.0/) -->

ライセンス/著作権: [CC BY-NC-ND 4.0](https://creativecommons.org/licenses/by-nc-nd/4.0/)

<!-- Note: This section is included in its original, unaltered form with permission under the terms of the [CC BY-NC-ND 4.0](https://creativecommons.org/licenses/by-nc-nd/4.0/) license. No changes have been made. -->

注: このセクションは、[CC BY-NC-ND 4.0](https://creativecommons.org/licenses/by-nc-nd/4.0/) ライセンスの条項に基づき、許可を得て原文のまま収録されている。変更は加えられていない。

---

<!-- Scrum thrives when people are willing to share what they see, even when it is incomplete, inconvenient, or uncomfortable. Speaking up should be the default, not the exception. Psychological safety creates an environment for meaningful inspection and adaptation, which is how Scrum delivers learning and enables high performance. -->

スクラムが真価を発揮するのは、人々が自分の見えていることを、それが不完全でも、不都合でも、言いにくいことであっても共有しようとするときである。発言することは例外ではなく、当たり前であるべきだ。心理的安全性は、意味のある検査と適応のための環境を生み出す。そして、それこそがスクラムに学習をもたらし、高パフォーマンスを可能にする。

<!-- ### The fear tax in Scrum Teams -->

### スクラムチームにおける恐れの代償 {#the-fear-tax-in-scrum-teams}

<!-- Many Scrum practitioners have observed this: Scrum events that appear to work on the surface but feel empty. Sprint Retrospective that ends with safe, low-impact actions or none at all. No one challenges the goal, work, or assumptions during Sprint Planning, and silence replaces candid disagreement. You might also recognize this in the avoidance of hard questions and crucial conversations. Or in moments where status overrides expertise: a less senior product developer notices a quality risk, but the discussion is dominated by a more senior voice. These are often treated as facilitation or communications issues, but they are early signs of something deeper. -->

多くのスクラム実践者には、心当たりがあるだろう：表面上はうまく回っているように見えるのに、どこか空虚なスクラムイベント。無難で影響の少ないアクション、またはまったくアクションなしで終わるスプリントレトロスペクティブ。スプリントプランニング中に誰もゴール、作業、または前提に異議を唱えず、率直な議論の代わりに沈黙が場を支配する。難しい問いや重要な会話が避けられている場面にも、同じことが表れているかもしれない。あるいは、地位が専門性を上回ってしまう瞬間にも見られる：ジュニアのプロダクト開発者が品質リスクに気づくが、議論はよりシニアな人の声に押し切られてしまう。これらはしばしばファシリテーションやコミュニケーションの問題として片付けられるが、もっと深刻な問題の初期症状であることが多い。

<!-- This is common. It is not an exception. Scrum Teams pay a fear tax every Sprint. This cost is invisible at first glance, but it accumulates over time. The fear tax is driven by concerns about blame, embarrassment, appearing incompetent, or losing status or popularity. Fear consumes people's capacity even before the work starts. It shows up in small, everyday choices people make to self-protect: withholding concerns, softening language, delaying bad news, avoiding certain topics, or not asking for help. Each choice seems harmless, and it often feels like the best decision in that moment. Together, those choices create a compounding effect that degrades learning and decreases performance, even though no single moment looks dramatic. Fear delays risk detection and course correction. Problems do not disappear; they move downstream. Ultimately, the fear tax is often borne by the customer. -->

これは珍しいことではない。例外でもない。スクラムチームは、スプリントごとに恐れの代償を払っている。このコストは一見見えないが、時間とともに蓄積される。恐れの代償を生み出すのは、非難されること、恥をかくこと、無能だと思われること、地位や人気を失うことへの不安である。恐れは、作業が始まる前から人々の能力を奪う。それは、日々の小さな自己防衛の選択として現れる：懸念を口にしない、言い方を和らげる、悪いニュースを先延ばしにする、特定のトピックを避ける、または助けを求めない。どの選択も一見、無害に思われ、その場では最善の決定のように感じられることが多い。だが、そうした選択が積み重なると、どの瞬間も劇的には見えなくても、学習を損ない、パフォーマンスを低下させる複合的な効果が生まれる。恐れは、リスクの発見と軌道修正を遅らせる。問題は消えるのではなく、後工程へ先送りされる。最終的に、恐れの代償を負担するのは、しばしば顧客である。

<!-- Scrum is based on the pillars of transparency, inspection, and adaptation[^1]. When fear is present, transparency becomes selective, inspection narrows to carefully framed updates, and adaptation remains superficial. Fear constrains empiricism – the ability to learn from what is actually happening. -->

スクラムは透明性、検査、適応という柱の上に成り立っている [^1]。恐れがあると、透明性は選択的になり、検査の範囲は慎重に整えられた更新に狭まり、適応は表面的なままに留まる。恐れは経験主義 - 実際に起こっていることから学ぶ能力 - を損なう。

<!-- Psychological safety (as defined by Amy Edmondson[^2]) is a capability Scrum Teams can develop and sustain to support learning and high performance. This work examines how psychological safety shows up in real Scrum work, how it affects learning and outcomes, and how Scrum Teams and leaders strengthen it through deliberate experiments in how they collaborate and learn from experience. For Scrum to be truly effective, it must create a safe space for learning. High performance emerges over time. -->

心理的安全性（Amy Edmondson [^2] の定義による）は、スクラムチームが学習と高パフォーマンスを支えるために育み、維持していける能力である。本書は、心理的安全性が実際のスクラムの仕事の中でどのように現れ、学習とアウトカムにどう影響し、そしてスクラムチームとリーダーが協働や経験からの学習の方法を意図的に実験しながら、どのように心理的安全性を強化するかを検討する。スクラムが真に効果的であるためには、学習のための安全な場が必要である。時間をかけて、高パフォーマンスが体現されていく。

<!-- ### What psychological safety is – and what it is not -->

### 心理的安全性とは何か - そして何ではないか {#what-psychological-safety-is-and-what-it-is-not}

<!-- According to Amy Edmondson, psychological safety is a shared belief that the team is safe for interpersonal risk-taking[^2]. An interpersonal risk is a risk someone takes when interacting with people. It means doing or saying something without knowing how others will react, for example, raising a hand in a meeting to admit you did not understand what was being discussed. Those reactions might range from supportive responses such as curiosity, attentive listening, and a willingness to help, to less supportive responses such as ignoring, blaming, or even assuming incompetence or questioning someone's credibility. Asking a question may be perceived as being uninformed or unprepared. Sharing a new idea may result in its dismissal or mockery rather than serious discussion. Admitting a mistake may lead to blame or shame, rather than to an invitation to explore why it happened. A team that is safe for interpersonal risk-taking is one in which people consistently feel that questions are welcome, ideas are thoughtfully considered, and mistakes are treated as opportunities to learn and improve, rather than as reasons for embarrassment, judgment, or punishment. -->

Amy Edmondsonによると、心理的安全性とは、このチームでは対人リスクを取っても安全であると、メンバーによって共有された信念である [^2]。対人リスクとは、人々と相互作用するときに誰かが取るリスクである。それは、相手がどのように反応するか分からないまま、何かをしたり言ったりすることを意味する。例えば、ミーティングで手を挙げて、議論の内容を理解できていなかったと認めることである。そうした行動に対する反応はさまざまだ。好奇心をもって聞く、丁寧に耳を傾ける、助けようとする、といった支援的な反応もあれば、無視する、非難する、能力を疑う、信頼性を疑問視するといった批判的な反応もある。質問をすることは、知識が足りない、または準備不足だと受け取られるかもしれない。新しいアイデアを共有しても、真剣に議論される代わりに、却下されたり、嘲笑されたりするかもしれない。間違いを認めたときも、なぜそれが起こったかを一緒に探索しようとはならず、非難や恥につながる可能性がある。対人リスクを取っても安全なチームとは、質問は歓迎され、アイデアは真剣に検討され、間違いは恥や批判や罰の理由ではなく学習と改善の機会として扱われる——メンバーがそう一貫して感じられるチームのことである。

<!-- The definition of psychological safety is empirical and research-based rather than aspirational. Psychological safety is not an individual trait. It is a team-level condition that forms over time through repeated experience of how others respond in different situations. It is not about comfort, niceness, or artificial harmony. When teams avoid disagreement or suppress difficult topics to preserve harmony, they prioritize comfort over psychological safety. Psychological safety enables constructive conflict, not its absence (see also Lencioni's model in [^3]). It is not a lack of accountability either. High psychological safety combined with high standards enables a learning and high-performance zone[^4]. In Scrum, high standards are expressed through clear expectations such as Definition of Output Done and Definition of Outcome Done, meaningful Sprint Goals, and accountability for outcomes. Google's Project Aristotle identified psychological safety as a key factor in team effectiveness[^5]. The learning zone is where Scrum Teams want to operate, because complex work requires learning. -->

心理的安全性の定義は理想論ではなく、研究に基づく実証的なものである。心理的安全性は個人の特性ではない。それはチームレベルの条件であり、様々な状況で他者がどう反応するかという繰り返しの経験を通じて、時間とともに形成される。それは快適さや当たり障りのなさ、または表面的な調和を意味しない。チームが表面的な調和を守るために意見の違いや難しいトピックを避けるとき、それは心理的安全性ではなく、快適さを優先していると言える。心理的安全性は建設的な対立を可能にするものであって、対立そのものをなくすものではない（Lencioniのモデル[^3] も参照）。それは説明責任がなくなることでもない。高い心理的安全性と高い基準が組み合わさると、学習と高パフォーマンスが両立するゾーンが生まれる [^4]。スクラムでは、高い基準はアウトプット完成の定義とアウトカム完成の定義、意味のあるスプリントゴール、アウトカムに対する説明責任などの明確な期待として現れる。Googleのプロジェクトアリストテレスでも、心理的安全性はチームの有効性を左右する主要な要因として特定された [^5]。複雑な仕事には学習が欠かせないからこそ、スクラムチームはこの学習ゾーンで働く必要がある。

<!-- Signs of psychological safety include: -->

心理的安全性の兆候には以下が含まれる：

<!-- - If I make a mistake, it will not be used against me. -->
<!-- - Speaking openly is expected. -->
<!-- - I can speak up, offer ideas, another point of view, and ask questions without fear of punishment or embarrassment. -->

- ミスをしても、それが自分に不利に使われない。
- 率直に発言することが期待されている。
- 罰や恥を恐れることなく、発言し、アイデアを別の視点で提供し、質問できる。

<!-- These beliefs are situational; they can vary across situations and over time, even within the same Scrum Team. For example, the Scrum Team might feel safe during Sprint Retrospectives but not during Sprint Reviews. -->

これらの信念は状況によって変わる。同じスクラムチームの中でも、状況や時間によって異なることがある。例えば、スクラムチームはスプリントレトロスペクティブでは安全と感じるが、スプリントレビューではそうではないかもしれない。

<!-- Psychological safety is created and reinforced through how people interact. It develops through everyday interaction patterns. It is sensitive to how people treat one another in moments of uncertainty. Because it is shaped by experience rather than intention, psychological safety can shift quickly; a single dismissive comment or unresolved incident can have lasting effects on what people feel safe to say. Managers and stakeholders have disproportionate influence because their words, reactions, and decisions signal what is acceptable. When people fear that they will contradict, offend, or disappoint a leader, they may hold back questions or concerns, even when doing so harms the work. This is why leaders should speak last. The influence is not limited to formal roles. Team members also shape safety through their responses to ideas, mistakes, and disagreements. -->

心理的安全性は、人々の相互作用を通じて作られ、強化される。それは日常の相互作用のパターンを通じて発展する。それは不確実な場面で人々が互いにどのように接するかに大きく影響される。心理的安全性は意図ではなく経験によって形成されるため、急速に変化することもある。たった一度の突き放すようなコメントや、放置された出来事が、ここで何を言っても安全と感じるかに長く影響を与えることがある。マネージャーとステークホルダーは突出した影響力を持っている。なぜなら、彼らの言葉、反応、決定が何が許容されるかを示すからである。リーダーに反論したり、不快にさせたり、失望させたりすることを恐れると、たとえ仕事を損なうとしても、質問や懸念を控える人もいるかもしれない。そのため、リーダーは最後に話したほうがよい。影響力は公式な役割に限定されない。チームメンバーもまた、アイデア、間違い、意見の違いに対する反応を通じて、安全性を形作っている。

<!-- ### Psychological safety in the context of Scrum -->

### スクラムのコンテキストにおける心理的安全性 {#psychological-safety-in-the-context-of-scrum}

<!-- Voluntary interpersonal risk-taking is a needed core element of Scrum. It reflects openness, courage, and transparency in Scrum by design, because work and decisions are made visible and critiqued within the Scrum Team. People don't come to work to look ignorant, incompetent, or disruptive. Neither do they plan intentional errors. However, when people speak up, ask questions, or admit mistakes, they risk how others perceive them and interpret their intentions. A common response to reduce those risks is silence: don't speak, don't ask questions, don't challenge the status quo, don't offer ideas, and don't admit mistakes. Silence becomes a form of self-protection. This pattern, known as impression management[^6], leads to missed opportunities for learning, innovation, and product and organizational improvement. In Scrum Teams, impression management often entails concealing problems or doubts to appear competent, confident, and in control, rather than speaking candidly about what is actually happening. -->

自発的に対人リスクを取ることは、スクラムの中核にある重要な要素である。スクラムでは、作業や意思決定が可視化され、チームの中で吟味されるため、設計上、公開性、勇気、透明性が前提となる。人々は仕事の場で、無知、無能、あるいは破壊的だと思われたくない。わざと失敗しようとしているわけではない。しかしながら、発言したり、質問したり、ミスを認めるとき、人は自分がどう見られているか、自分の意図がどう受け止められるかについてリスクを負う。こうしたリスクを避けるためのもっとも一般的な反応は沈黙である：発言しない、質問しない、現状に異議を唱えない、アイデアを出さない、ミスを認めない。沈黙は自己防衛の手段になる。印象管理 [^6] として知られるこのパターンは、学習、イノベーション、プロダクトや組織の改善の機会を逃すことにつながる。スクラムチームでは、印象管理は、実際に何が起こっているかについて率直に話す代わりに、有能で、自信があり、状況を把握しているように見せようとして、問題や疑念を隠してしまうことが多い。

<!-- Scrum Teams often face interpersonal risks during formal events, informal meetings, or conversations. Those are the moments when Scrum Team members ask themselves, "Should I speak up or stay silent?" In Scrum, this internal dilemma shows up in concrete, specific situations: -->

スクラムチームは、公式なイベントでも、非公式なミーティングでも、何気ない会話の中でも、しばしば対人リスクに直面する。そうした瞬間に、スクラムチームメンバーは「ここで発言すべきか、沈黙すべきか？」と自問する。スクラムでは、この内部の葛藤が、次のような具体的な場面で現れる：

<!-- - **Reaction to Mistakes:** When a mistake or quality issue is noticed during the Daily Scrum, Sprint Retrospective, or Sprint Review, the team acknowledges it publicly. Instead of quietly fixing it in the background, they talk about it, understand it, and resolve it. More is the pity, as a focus on reducing errors leads to fewer insights[^7]. -->

- **間違いへの反応：** デイリースクラム、スプリントレトロスペクティブ、またはスプリントレビューのなかで、間違いや品質上の問題に気づいたとき、チームがそれを公に認めるかどうか。裏で静かに修正する代わりに、話し合い、理解し、解決する。残念なことに、エラーを減らすことに目を向けすぎると、かえって洞察が得られなくなる [^7]。

<!-- - **Dealing with Issues:** When work becomes difficult during the Sprint, and impediments need to be surfaced early in the Daily Scrum rather than hidden to preserve the appearance of progress. -->

- **問題への対処：** スプリント中に作業が困難になったとき、見せかけの進捗を取り繕うために隠すのではなく、デイリースクラムで早期に障害を表面化させられるかどうか。

<!-- - **Embracing Diversity:** When product assumptions, decisions, or technical approaches are challenged during Sprint Planning or Backlog Refinement, especially when that challenge comes from someone with less formal authority or seniority. -->

- **多様性を受け入れる：** スプリントプランニングやバックログリファインメントで、プロダクトに関する前提や判断、技術的アプローチに異議が唱えられたとき、それが年次や役職の低い人からの指摘であっても受け止められるかどうか。

<!-- - **Taking Risks:** When Scrum Teams are encouraged to run experiments, technical spikes, or discovery work where outcomes are uncertain, and learning may show up as "no, not this path" rather than visible success. -->

- **リスクを取る：** アウトカムが不確実で、学習が目に見える成功としてではなく、「この道ではなかった」という形で現れる場合でも、実験、技術的スパイク、またはディスカバリーの作業をスクラムチームが進んで行えるかどうか。

<!-- - **Asking for Help:** Asking for help, pairing, or clarification can expose gaps in understanding to peers or stakeholders. -->

- **助けを求める：** 自分の理解不足が同僚やステークホルダーに分かってしまう場面でも、助けやペア作業、説明を求めることができるか。

<!-- - **Mutual Support:** When supporting a teammate under pressure means sharing responsibility for outcomes rather than protecting individual credibility (*mutual support*). -->

- **相互支援：** プレッシャー下のチームメイトをサポートするのは、自分への評価を守るからではなく、アウトカムに対する責任を分かち合うためかどうか（*相互支援*）。

<!-- - **Appreciation:** When contributing expertise or effort that improves long-term product quality or team effectiveness, knowing that this contribution may not be immediately visible or rewarded. -->

- **感謝：** すぐに認められなかったり報酬に繋がらない場合でも、長期的なプロダクト品質やチームの有効性を高める専門知識や取り組みに貢献できるかどうか。

<!-- These situations are not edge cases; they are everyday moments where psychological safety is either strengthened or diminished. The seven behavioral patterns named above are consistent with the Team Psychological Safety assessment vocabulary[^8]. -->

こうした場面は特別なケースではない。心理的安全性が詰まるか、弱まるかが決まる日常の瞬間である。ここで挙げた7つの行動パターンは、チーム心理的安全性評価の語彙と整合している [^8] 。

<!-- Scrum does not remove interpersonal risks. It makes them transparent. Psychological safety determines whether these moments become sources of learning and improved performance or reasons for self-protection. Because Scrum relies on frequent inspection, adaptation, and collective problem-solving, withholding effort directly limits Scrum's effectiveness. -->

スクラムは対人リスクを取り除くわけではない。むしろ、それらを可視化する。そうした瞬間が、学習とパフォーマンス向上の機会になるのか、それとも自己防衛の引き金になるのかを左右するのが、心理的安全性である。スクラムは頻繁な検査、適応、そして協働による問題解決に依存している。だからこそ、懸念や気付きを差し控えることは、スクラムの有効性を直接損なう。

<!-- How teams respond to errors is a critical aspect of psychological safety in the context of Scrum. Product Developers are accountable for instilling quality by adhering to a Definition of Output Done[^9]. People make mistakes for different reasons, especially in complex work. Psychological safety does not mean tolerating repeated avoidable mistakes or reducing professionalism. Instead, it creates an environment in which team members feel safe being transparent about errors, the first step toward learning and improvement. Not all failures are the same, and responding to them requires judgment. Amy Edmondson defines 3 types of failures[^10]: -->

チームがエラーにどのように反応するかは、スクラムのコンテキストにおいて、心理的安全性を考えるうえで極めて重要である。プロダクト開発者は、アウトプット完成の定義を遵守することによって品質を作り込むことに説明責任を負う [^9]。しかし、特に複雑な作業では、人はさまざまな理由でミスをする。心理的安全性は、繰り返し起こる避けられるミスを容認することでも、プロフェッショナリズムを損なうことでもない。そうではなく、チームメンバーが、エラーについて率直に話すことを安全に感じる環境を作り出す。これは学習と改善への第一歩である。とはいえ、すべての失敗が同じではない。どう向き合うべきかは、失敗の種類によって異なる。Amy Edmondsonは、失敗を次の3種類に分けている [^10]：

<!-- - **Basic failures:** Knowledge is well developed, and uncertainty is low. For example, misconfiguring a standard deployment pipeline or forgetting to follow a known test procedure. -->

- **基本的な失敗：** 知識は十分にあり、不確実性も低い状況で起こる失敗。例えば、標準的なデプロイパイプラインの設定ミスや、既知のテスト手順に従うことを忘れる、といったもの。

<!-- - **Complex failures:** Knowledge is well-developed, vulnerable to unexpected events, and uncertainty is moderate. For example, a production outage may be caused not by a single mistake but by a chain of smaller issues, or multiple teams may each make the most logical local decision, only to discover later that their choices conflict during integration. -->

- **複雑な失敗：** 知識は十分にあるが、予期しない出来事の影響を受けやすく、不確実性が中程度である状況で起こる失敗。例えば、単一のミスではなく、より小さな問題の連鎖によって引き起こされるような本番環境の停止や、複数のチームがそれぞれは最も合理的な判断をしたにもかかわらず、統合時になって整合性が取れていないことが判明する、といったもの。

<!-- - **Intelligent failures:** Knowledge is limited, and uncertainty is high. For example, running a controlled experiment to validate a hypothesis that turns out to be wrong or attempting a novel technical approach that does not produce the expected performance. -->

- **知的な失敗：** 知識がまだ限られており、不確実性が高い状況で起こる失敗。例えば、仮説を検証するために実験した結果、その仮説が間違っていることが判明する、または新しい技術的アプローチを試したものの期待したパフォーマンスが得られなかった、といったもの。

<!-- Psychological safety supports open discussion and learning from failures (or errors) that arise from uncertainty and exploration, whereas Scrum Teams openly discuss them and prevent the same avoidable mistakes from recurring. In that sense, the only true failure the Scrum Team faces is failing to learn and apply what was learned. The prime directive for Retrospectives is expressing one of the fundamental elements related to psychological safety – reaction to errors: "Regardless of what we discover, we understand and truly believe that everyone did the best job they could, given what they knew at the time, their skills and abilities, the resources available, and the situation at hand"[^11]. -->

心理的安全性は、不確実性と探索から生じる失敗（またはエラー）について、オープンに議論し、そこから学習することを可能にする。スクラムチームはそれらをオープンに議論し、同じような避けられるミスが再発することを防ぐ。その意味で、スクラムチームにとって本当の失敗は、失敗そのものではなく、そこから学習せず、学んだことを適用しないことである。レトロスペクティブの原理原則は、心理的安全性の中核である - エラーへの反応 - をよく表している：「レトロスペクティブでどんな事実が明らかになろうとも、その時点で知り得たこと、持っていたスキルや能力、利用可能なリソース、そして置かれていた状況のなかで、皆ができる限り最善の仕事をしたと、私たちは理解し、心からそう信じる」[^11]。

<!-- ### Scrum pillars, Scrum values, and psychological safety in practice -->

### スクラムの柱、スクラムの価値基準、そして実践における心理的安全性 {#scrum-pillars-scrum-values-and-psychological-safety-in-practice}

<!-- When discussing the connection between psychological safety and Scrum, a common question arises: do Scrum values create psychological safety, or does psychological safety enable Scrum values? Do Scrum pillars lead to safety, or does safety enable them? The more useful question is not which comes first (the chicken-or-egg dilemma), but how these elements reinforce or weaken one another over time. As Scrum is an empirical social system, it is worth examining how these conditions evolve through feedback loops created by Scrum events. This distinction matters because Scrum Teams often try to change behavior without examining how the system itself shapes it. -->

心理的安全性とスクラムの関係を議論するとき、よく出てくる問いがある：スクラムの価値基準が心理的安全性を作り出すのか、それとも心理的安全性があるからこそ、スクラムの価値基準が実現されるのか？スクラムの柱は安全性をもたらすのか、それとも安全性があるからこそ柱が機能するのか？だが、より重要なのは、どちらが先か（鶏が先か卵が先かのジレンマ）ではなく、これらの要素が時間とともにどのように互いを強化、または弱体化するかである。スクラムは経験主義に基づく社会的なシステムであるため、スクラムイベントが生み出すフィードバックループを通じて、こうした条件がどのように進化するかを検討する価値がある。この視点が重要なのは、スクラムチームはしばしば、システム自体が行動をどのように形作っているかを問うことなく、行動だけを変えようとするからである。

<!-- The empirical Scrum pillars of transparency, inspection, and adaptation[^1] increase visibility and create opportunities for learning in Scrum Teams: -->

スクラムの経験主義を支える柱である透明性、検査、適応 [^1] は、仕事を見える化し、スクラムチームに学習の機会を作り出す：

<!-- - Transparency exposes work, progress, assumptions, mistakes, and uncertainty. -->
<!-- - Inspection invites questioning, challenge, and evaluation. -->
<!-- - Adaptation requires acknowledging that previous decisions were incomplete or incorrect, not due to fault but to limited information and uncertainty. -->

- 透明性は作業、進捗、前提、ミス、不確実性を表に出す。
- 検査は質問、異議、評価を促す。
- 適応は、以前の判断が不完全または不正確であったことを認めることを求める。それは誰かの過失ではなく、限られた情報と不確実性による。

<!-- From that perspective, each Scrum pillar increases interpersonal risk. Speaking openly, admitting uncertainty, or challenging direction all happen publicly, in front of others. Thus, Scrum, by design, puts people in situations where social exposure is unavoidable. How teams respond to that exposure is where Scrum values come into play. -->

この観点から見ると、スクラムの各柱は対人リスクを高める。オープンに発言すること、不確実性を認めること、または方向性に異議を唱えることは、すべて人前で行われるからだ。つまりスクラムは設計上、人を社会的な露出が避けられない状況に置く。その露出にチームがどう反応するかを方向づけるのが、スクラムの価値基準である。

<!-- Scrum as a framework does not create fear. Whenever people work closely with others, interpersonal risk is always present. Scrum reveals how teams respond to interpersonal risk and creates formal opportunities, through Scrum events, to reflect on and improve those responses. -->

スクラムというフレームワークが恐れを生み出すわけではない。人が他者と密接に働く以上、対人リスクは常に存在する。スクラムはチームが対人リスクにどのように反応するかを明らかにし、スクラムイベントを通じて、それらの反応を振り返り改善するための公式の機会を作り出す。

<!-- The five Scrum values – commitment, focus, openness, respect, and courage – do not eliminate interpersonal risk-taking. They shape how Scrum Teams respond when it shows up[^12]: -->

スクラムの5つの価値基準 - 確約、集中、公開、尊敬、勇気 - は対人リスクそのものをなくすわけではない。むしろ、それらが現れたときに、スクラムチームがどう反応するかを方向づける [^12]：

<!-- - **Openness** supports sharing incomplete or uncomfortable information. -->
<!-- - **Respect** reduces the social cost of speaking up and offering diverse perspectives, and curtails bluntness disguised as 'openness.' -->
<!-- - **Courage** supports challenge and dissent despite uncertainty. -->
<!-- - **Commitment** shifts attention from self-protection to a shared goal. -->
<!-- - **Focus** prevents noise and personal agendas from dominating the discussion. -->

- **公開** は不完全または不快な情報の共有を後押しする。
- **尊敬** は発言したり多様な視点を持ち込むことの社会的コストを減少させ、「公開」を装った無神経さを抑制する。
- **勇気** は不確実であっても異議を唱え、反対意見を述べることを後押しする。
- **確約** は自己防衛ではなく、共有された目標に注意を向ける。
- **集中** は雑音や個人的な思惑が議論を支配することを防ぐ。

<!-- When these values are lived, interpersonal risk becomes manageable and creates opportunities for learning: what to improve, whether to pivot, and what to do next – about product decisions, quality, and ways of working. -->

これらの価値が実践されるとき、対人リスクは扱えるものになり、学習の機会が生まれる：何を改善するか、ピボットすべきかどうか、次に何をすべきか -- プロダクトの意思決定、品質、働き方について。

<!-- Psychological safety is not a value, a rule, or an intention. It is a belief that forms over time, based on what actually happens when people take interpersonal risks: when someone admits a mistake, when assumptions are challenged, and when bad news is delivered early. When the consequences are constructive, psychological safety increases. When the consequences are punitive, dismissive, or humiliating, psychological safety decreases, regardless of declared values. In this sense, psychological safety is an emergent property of how Scrum pillars and values are enacted in practice. Therefore, psychological safety becomes a functional requirement for Scrum to work as intended. -->

心理的安全性は価値でも、ルーででも、意図でもない。それは、人々が対人リスクを取るときに実際に何が起こるかに基づいて、時間とともに形成される信念である：誰かがミスを認めるとき、前提に疑問が投げかけられたとき、悪い知らせが早めに共有されたとき。その結果が建設的であれば、心理的安全性は高まる。逆に、結果が懲罰的、軽蔑的、または屈辱的であるとき、どれほど価値を掲げていていようとも、心理的安全性は低下する。この意味で、心理的安全性はスクラムの柱と価値基準がどう実践されるかによって生まれる創発的な性質だと言える。したがって、心理的安全性は、スクラムが意図したとおりに機能するための実質的な要件となる。

<!-- Scrum pillars, values, and psychological safety co-evolve, forming a reinforcing loop: -->

スクラムの柱、価値基準、心理的安全性は、互いに影響し合いながら進化し、強化ループを形成する：

<!-- - Scrum pillars expose interpersonal risk. -->
<!-- - Scrum values shape responses to that risk. -->
<!-- - Those responses form psychological safety. -->
<!-- - Psychological safety determines whether transparency, inspection, and adaptation remain real. -->

- スクラムの柱は対人リスクを可視化する。
- スクラムの価値基準がそのリスクへの反応を形作る。
- その反応の積み重ねが心理的安全性を形成する。
- 心理的安全性は、透明性・検査・適応が形骸化せずに機能し続けるかを左右する。

<!-- When this loop is reinforcing, Scrum supports sustained learning and enables high-performing Scrum Teams. When it is broken, Scrum degrades, and its benefits are diminished over time through everyday interactions and decisions. This is why psychological safety cannot be treated as a side concern. -->

このループが強化されているとき、スクラムは持続的な学習を促し、スクラムチームは高いパフォーマンスを実現する。逆にこのループが壊れているとき、スクラムは形骸化し、日々のやり取りや決定を通じて時間とともにその価値が失われる。だからこそ、心理的安全性を後回しにすることはできない。

<!-- ### Psychological safety as learning infrastructure in Scrum Teams -->

### スクラムチームにおける学習の基盤としての心理的安全性 {#psychological-safety-as-learning-infrastructure-in-scrum-teams}

<!-- Scrum was designed to help people, teams, and organizations generate value through adaptive solutions for complex problem domains[^1]. It operates in conditions of uncertainty, where sustained performance depends on effective continuous learning and shared sense-making rather than perfect execution. Effective learning requires early exposure to uncertainty, incomplete understanding, weak signals, and emerging risks – before they lead to costly decisions made without sufficient insight. Psychological safety enables people to speak up before certainty exists – when learning still has the greatest leverage. When psychological safety supports speaking up, assumptions are challenged early, problems are surfaced while options remain open, and learning happens when change is still relatively inexpensive and course-correction opportunities remain available. Delayed understanding leads to late problem detection, fewer adaptation options, and the accumulation of hidden product, technical, and decision risks that remain out of sight. -->

スクラムは、人、チーム、組織が、複雑な問題領域に対する適応的な解決策を通じて価値を生み出せるよう設計されている [^1]。そこで前提となるのは不確実性であり、持続的なパフォーマンスは、完璧な実行よりも、効果的な継続的学習と共有されたセンスメイキングの形成にかかっている。効果的な学習には、十分なインサイトなしに高コストな判断を下してしまう前に、不確実性、不完全な理解、弱いシグナル、立ち上がりつつあるリスクに気づけることが必要である。心理的安全性は、確実な答えが出揃う前に - 学習の効果が最も大きい段階で - 人々が声を上げることを可能にする。心理的安全性が発言を後押しすれば、前提は早い段階で問い直され、まだ選択肢が残っているうちに問題が表面化し、変更コストがまだ比較的小さく、軌道修正の余地があるうちに学習できるのである。逆に、理解が遅れれば、問題発見も遅れ、適応の選択肢は減り、プロダクト、技術、意思決定の見えないリスクが蓄積されていく。

<!-- High performance in Scrum emerges over time through accurate inspection, timely adaptation, and repeated learning cycles. Psychological safety is not an objective for Scrum Teams; it is an enabling condition for the learning that leads to high performance. In that sense, psychological safety functions as infrastructure for delivering high value in an effective way: it allows learning to be reliable and sustained over time, rather than episodic or accidental. Because psychological safety can be observed and assessed across multiple dimensions, Scrum Teams can see whether this infrastructure is strengthening or weakening. Like any form of infrastructure, it is rarely noticed when it works well, but when it diminishes, it limits what Scrum Teams can achieve. This infrastructure emerges and evolves through everyday interactions and decisions. -->

スクラムにおける高パフォーマンスは、正確な検査、タイムリーな適応、繰り返される学習サイクルを通じて、時間をかけて体現されていく。心理的安全性はスクラムチームの目標ではない。それは高パフォーマンスにつながる学習を可能にする条件である。その意味で、心理的安全性は、高い価値を効果的に提供するための基盤として機能する：学習を断続的・偶発的なものではなく、継続的で信頼できるものにする。心理的安全性は複数の観点から観察および評価できるため、スクラムチームはこの基盤が強化されているか弱体化しているかを見ることができる。どんな基盤でもそうであるように、うまく機能しているときはほとんど気づかれないが、それが弱体化すると、スクラムチームが達成できることを制限してしまう。この基盤は、日常のやり取りと決定を通じて創発し進化する。

<!-- ### How leadership signals shape psychological safety -->

### リーダーシップのシグナルが心理的安全性をどのように形作るか {#how-leadership-signals-shape-psychological-safety}

<!-- Psychological safety is shaped by what the system consistently signals as acceptable more than by what people say they value. In Scrum contexts, this system comprises decision-making structures, feedback loops, incentives, and interaction norms that enable how people raise concerns, challenge assumptions, or acknowledge uncertainty. For example, whether insights from the Sprint Retrospective lead to meaningful decisions and change, or whether missed Sprint Goals trigger reflection or blame. -->

人々が口に出して価値があると言うことよりも、システムが一貫して許容可能として示すものが心理的安全性を形作る。スクラムのコンテキストでは、そのシステムは意思決定の構造、フィードバックループ、インセンティブ、および相互作用の規範から成り立つ。この規範は、人々が懸念を示したり、前提に疑問を投げかけたり、不確実性を認めたりする際の振る舞いを形作る。例えば、スプリントレトロスペクティブから得られたインサイトが、実際の意思決定や変化につながるかどうか、あるいは達成されなかったスプリントゴールが振り返りを促すのか、それとも非難を引き起こすか、といったものだ。

<!-- Managers and stakeholders have disproportionate influence because they control or strongly affect consequences such as approval, recognition, escalation, and how outcomes are interpreted – including what counts as success. How they respond in moments of uncertainty, error, or dissent sends a signal to everyone watching, including those who stay silent. When mistakes are met with curiosity and analysis, people learn they can speak up about them. When challenges are dismissed, ignored, or subtly penalized (such as being excluded from future discussions), people learn to withhold, even when no explicit blame is issued. Silence is often rational or emotional self-protection, not disengagement, because people are paying attention to the system's signals. This effect is amplified by status, hierarchy, seniority, and real or perceived expertise. In collective decision-making settings, lower-influence or less senior roles entail greater interpersonal risk when they question assumptions or raise concerns. If those contributions are consistently dismissed or minimized, expertise is suppressed, and learning degrades over time. -->

マネージャーとステークホルダーは突出した影響力を持つのは、承認、評価、エスカレーション、およびアウトカムの解釈 - 何が成功とみなされるかを含む - などの結果を左右したり、強い影響を持つからだ。不確実性、エラー、反対意見が生じる場面での彼らの反応は、黙って見ている人も含め、その場にいる全員にシグナルを送る。ミスが好奇心と分析で受け止められるとき、人々はそれについて発言できると学ぶ。異議が却下、無視、または微妙な形で罰せられるとき（例えば将来の議論から外されるなど）、明示的な非難がなくても、人々は差し控えることを学ぶ。沈黙は、無関心なのではなく、しばしば合理的または感情的な自己防衛である。人々はシステムが発するシグナルに注意を払っているからだ。この効果は、地位、階層、年功序列、そして実際のあるいは認識されている専門知識によって更に強まる。集団で意思決定する場では、影響力の弱い立場やジュニアの人ほど、前提に疑問を投げかけたり懸念を提起したりするときに、より大きな対人リスクを伴う。そうした貢献が一貫して却下または軽視されると、専門知識は抑制され、学習の質も次第に下がっていく。

<!-- Leadership influence is not limited to formal roles. Experienced Product Developers, Scrum Masters, and Product Owners act as informal leaders through facilitation choices, reactions to tensions, and responses to dissent. Non-intervention is also a signal – often the strongest one. When dismissive behaviour goes unaddressed, the system quietly teaches what is unsafe to say. -->

リーダーシップの影響力は公式の役割に限定されない。経験豊富なプロダクト開発者、スクラムマスター、プロダクトオーナーもまた、ファシリテーションの選び方、緊張が高まった場面への応じ方、反対意見への向き合い方を通じて、非公式なリーダーシップを発揮している。何もしないこともまた、一つのシグナルである -- しばしば最も強いものである。見下すようなふるまいが放置されると、システムは何を言うと危険なのかを静かに教えてしまう。

<!-- Leaders can foster psychological safety, but their work is never done. It is sustained through continual practice. Building and reinforcing the work environment where people can learn, innovate, and grow is an ongoing work[^4]. Because psychological safety is shaped through everyday interactions, it can be strengthened through deliberate actions rather than cultural slogans. And it starts with small choices. -->

リーダーは心理的安全性を育むことができるが、その仕事に決して終わりはない。それは継続的な実践を通じて維持される。人々が学習し、イノベーションを起こし、成長できる職場環境を作り、育て続ける必要がある [^4]。心理的安全性は日常の相互作用を通じて形作られるため、文化的なスローガンではなく意図的な行動を通じて強化できる。そしてその出発点は、日々の小さな選択である。

<!-- ### Inspecting the conditions for learning -->

### 学習の条件を検査する {#inspecting-the-conditions-for-learning}

<!-- Scrum requires transparency to enable inspection and adaptation. If something is not visible, the Scrum Team cannot meaningfully change it. The same principle applies to psychological safety, and the whole team shares responsibility for inspecting it. When teams assume safety based on intent, values statements, or the absence of visible conflict, they lose the ability to inspect how their system actually behaves. -->

スクラムは、検査と適応を可能にするために透明性を必要とする。見える化されていなければ、スクラムチームは意味のある形で変えることができない。同じ原則が心理的安全性にも当てはまり、チーム全体がそれを検査する責任を共有する。善意や掲げている価値観、表面上の対立がないことを理由に安全性が高いと思い込んでしまうと、システムが実際にどのように振る舞うかを検査する能力を失ってしまう。

<!-- Scrum events make team behavior visible. Who speaks up during Sprint Planning? What is raised – and what is avoided – in the Daily Scrum? Which assumptions are challenged in Sprint Review discussions? What is named, and what is softened, in the Sprint Retrospective? These are observable signals, not opinions. By treating psychological safety as an inspectable condition rather than a cultural label, Scrum Teams can examine where transparency leads to learning and where it breaks down. Silence, politeness, or quick alignment are not conclusions; they are data points. Interpreted through inspection, they reveal how the team responds to uncertainty, error, disagreement, and risk. -->

スクラムイベントはチームのふるまいを可視化する。スプリントプランニング中に誰が発言するか？デイリースクラムで何が提起され、何が避けられるか？スプリントレビューの議論では、どの前提に疑問が投げかけられているか？スプリントレトロスペクティブでは、何が率直に名指しされ、何が柔らかく言い換えられているか？こうしたものは意見ではなく、観察可能なシグナルである。心理的安全性を文化的なラベルではなく、検査可能な条件として扱うことで、スクラムチームは、どこで透明性が学習につながり、どこでそれが崩壊するかを見て取れる。沈黙、礼儀正しさ、あるいは早すぎる意見の一致、それ自体は結論ではない。あくまでデータポイントである。それらを検査の対象として捉えることで、チームが不確実性、エラー、意見の違い、リスクにどのように反応するかが見えてくる。

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
