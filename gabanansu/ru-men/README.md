# 入門

### 概要

Euler Protocolのコードは、Ethereumネットワーク上のオンチェーンガバナンスを通じて、分散型コミュニティによって制御されています。コミュニティはEUL（オイル）と呼ばれるプロトコルネイティブなガバナンストークンを保有しており、コミュニティがEuler Protocolのコードに変更を加えることを可能にしています。トークンは、プロトコルのアップグレードを提案したり、他の人の提案に投票するために使用することができます。

### プロトコルコード

ガバナンスは、以下のようなパラメータについて、Euler上で変化をもたらすための投票を行うことができます。

1. デフォルトのisolated層借入係数
2. 特定資産の担保・借入要因
3. cross層およびcollateral層への資産の組み入れ
4. リスクパラメータの選択と一般的な手法の変更

オンチェーンガバナンスは、投票権や提案権の委譲、タイムロックエグゼキュータによるプロトコル（およびガバナンス設定）の更新など、ユニークな機能を可能にします。これにより、プロトコルは進化する市場環境に適応し、プロトコルのコア部分を時間をかけてアップグレードすることができます。 一方、オフチェーンガバナンスについては、そのような見直すべきコードや実装はありません。

主に、Eulerにアクションを実行するよう呼びかけるものです。例えば、助成金の発行や請求書の支払いなどです。このように、主にコミュニティと協力して難しい決定を下す際に、Eulerを支援するために使用されます。 Eulerのプロトコルは、オンチェーン投票に [Tally](https://www.tally.xyz/governance/eip155:1:0xd8E2114f6bCbaee83CDEB1bD6650a28BBcF144D5) ガバナンスインターフェースを使用しています。一方、 [Snapshot](https://snapshot.org/#/eulerdao.eth/proposal/0x3b4b7e79c40df6860e7d612bdccc4969753e283dfd84673dc5fc4d201abcb317) は、オフチェーンまたは「ガスレス」投票に使用されるインターフェースです。

### プロセス

[General Governance Process](https://forum.euler.finance/t/welcome-to-the-euler-governance-forum/7)は、Governance Forumで文書化されています。

ガバナンスの流れは以下の通りです。

1. &#x20;[Euler Discord](https://discord.gg/CdG97VSYGk) の<mark style="color:blue;">#governance</mark> **チャンネル**でアイデア・案を議論する。
2. [RFC (Request For Comment) Proposal](https://forum.euler.finance/c/rfc-request-for-comment/11) のドラフトを作成し、Governanceフォーラムに提案し、さらなるフィードバックを得る。
3. ガバナンスフォーラムで [eIP (Euler Improvement Proposal)](https://forum.euler.finance/c/eip/5) を作成するには、フォーラムのモデレーターにご連絡ください。
4. [Snapshot](https://snapshot.org/#/eulerdao.eth) で作成されたeIP（オフチェーン投票 これはすべての種類の提案に必要なステップであり、提案が成功した場合、実行はEuler Foundationによって行われます。
5. _オプションのステップ -_ [_Tally_](https://www.tally.xyz/governance/eip155:1:0xd8E2114f6bCbaee83CDEB1bD6650a28BBcF144D5) _上で作成されたeIP（オンチェーン投票） 提案にスマートコントラクトの変更が含まれている場合のみ、スナップショット投票の後、Tally上で投票が行われます。提案が成功した場合、Eulerプロトコルのスマートコントラクトをターゲットに実行される。_

注目すべきは、プロトコルスマートコントラクトに拘束的または非拘束的なすべてのオフチェーン提案が、オフチェーンの「ガスレス」投票の結果次第で、ガスコスト削減のためにオンチェーン提案を持つことになるとは限らないことです。

一方、すべてのオンチェーン提案がオフチェーンの対応策を必要とするわけではありません。 オフチェーン投票の結果によっては、オンチェーン提案が作成され、成功すればターゲットプロトコルのスマートコントラクトに対して実行されるかもしれません。&#x20;

オフチェーン提案が、プロトコルスマートコントラクトに対して実行されるオンチェーン提案を必要とする場合、一般的な流れは次のようになります。 Governanceフォーラムで正式なIdea/Proposalを作成して議論 → SnapshotでProposal作成（オフチェーン提案作成） → Off-Chain Voting →（オンチェーンガバナンスが必要な場合）フォーラムモデレーターがGovernanceフォーラムでeIP（Euler Improvement Proposal）作成 → TallyでeIP作成（オンチェーン提案作成） → オンチェーン投票（成功した場合、対象Eulerプロトコルのスマートコントラクトで実行される）

#### アイデア

ガバナンスの提案の可能性について議論を始めるには、フォーラムウェブサイトのアイデアセクションが最適な場所です。あなたのアイデアがコミュニティに関連し、よく練られていると確信が持てたら、ガバナンス・フォーラムに向かい、あなたのアイデアをめぐってコミュニティと議論を始めてください。（[forum](https://forum.euler.finance/t/welcome-to-the-euler-governance-forum/7)に記載されているプロセスに従ってください）

アイデアに関する議論やコメントが始まったら、コミュニティに積極的に働きかけ、提案に耳を傾けてください。通常、eIPになるまでに、コメント要求が成熟するのに1週間かかります。

#### ガバナンスプロポーザル

議論が十分に行われ、コミュニティが提案を明確に理解し、あなたのアイデアを支持した場合、（オンチェーン提案の場合）モデレーターによって、eIP：Euler Improvement Proposalとしてガバナンスカテゴリーに移動されます。提案にeIPが付くと、 [Tally governance dashboard](https://www.tally.xyz/governance/eip155:1:0xd8E2114f6bCbaee83CDEB1bD6650a28BBcF144D5)または [Snapshot governance dashboard](https://snapshot.org/#/eulerdao.eth/proposal/0x3b4b7e79c40df6860e7d612bdccc4969753e283dfd84673dc5fc4d201abcb317)でオンチェーンまたはオフチェーンの提案を作成することができます。 タリーやスナップショットの提案は、必ずしもeIPの作成者/提案者が作成する必要はなく、EULの最低基準値が満たされていない場合には、他の人物や代理人が投稿することができます。 グッドガバナンス提案の例は、こちらでご覧いただけます：eIP: WBTCを担保レベル3に昇格させる。  [community newsletter](https://newsletter.euler.finance/) を購読し、 [Twitter Page](https://twitter.com/eulerfinance)をフォローして、常に最新の情報を入手しましょう。
