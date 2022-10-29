# プロポーザルを書く

#### About

このガイドでは、まずフォーラムでガバナンスの提案を書き始め、その後Snapshot（オフチェーン）またはTally（オンチェーン）で提案を行う方法を説明します。

#### Step-by-step

フォーラムのRFC（Request for Comment）セクションは、ガバナンスの提案を作成するための最初のステップです。 [Euler Governance Forum](https://forum.euler.finance) の [RFC section](https://forum.euler.finance/c/rfc-request-for-comment/11) に移動して、新しい提案を作成します。よく練られたものであることを確認し、コミュニティと積極的に関わり、彼らのコメントに参加し、提案を受け入れるようにしましょう。

一貫性を持たせるために、以下のような提案構成をお勧めします。

#### Proposal Structure <a href="#proposal-structure-5" id="proposal-structure-5"></a>

* **Title:** \[プロポーザル名を入力してください。]
* **Author(s):** \[関連著者名を入力する]
* **Related Discussions:** \[リンクを貼る]
* **Submission Date:** \[日付の入力]

**Body Paragraphs/Sections:**

* **Simple Summary**: あなたの提案について、2-3文以内で簡潔に説明してください。
* **Abstract**: 提案の紹介と拡大 その提案が、ステークホルダー/トークン保有者の経験、プロトコルの性能、および全体的な導入プロセスをどのように改善するかについて、重要なポイントを強調する。
* **Motivation**: この提案はどのような問題を解決するのか？付加価値は何か？
* **Specification**: プロトコルに関連する質問に答える。

1. eIPの作成者と資産の関連性は？
2. 資産の簡単な説明を記入してください。
3. 資産の主な用途は？
4. なぜeIPがオイラーのエコシステムに利益をもたらすのか、説明してください。&#x20;
5. その資産はどこで取引されていますか？&#x20;
6. 取引量と時価総額はどの程度ですか？&#x20;
7. Uniswap V3流動性プールにおける流動性はETHに対してどのようなものですか？&#x20;
8. どのようなセキュリティ/監査レポートが行われていますか？

* **Implementation**: 提案書トランザクション生成ツールを用いて、提案書の実装を提示する。 [proposal transaction generation tool](https://proposal.euler.finance/).
* **Risk Assessment**: 提案に関わるリスクパラメータの評価を行う。

1. オラクルリスク&#x20;
2. 集中化リスク&#x20;
3. ボラティリティリスク
4. 流動性リスク&#x20;
5. スマートコントラクトのリスク

* **Voting**: 「賛成」「反対」投票の内容を定義してください。この提案に関連するスナップショット投票やフォーラムでの投票がある場合は、それらを添付してください。
* **Relevant Links**: EulerのOracleグレーディングツールや他のツール/リファレンスを使用した場合は、ここに追加してください、例えば 'Oracle グレーディングツール: [https://oracle.euler.finance/](https://oracle.euler.finance/)’

_グッドガバナンス提案書の例はこちらでご覧いただけます_。_:_ [eIP: Promote WBTC to collateral tier](https://forum.euler.finance/t/eip-1-promote-wbtc-to-collateral-tier/27)

2\. ガバナンスプロポーザル (オンチェーン or オフチェーン)

RFCがよく練られ、コミュニティがその提案を明確に理解し、あなたのRFCを支持した場合、その提案はmodによってeIP: Euler Improvement Proposalとしてガバナンスカテゴリに移されます。提案がRFCからeIPの段階に移されるには、通常1週間（7日）かかりますので、ご注意ください。eIPが割り当てられると、このeIPを使用してSnapshotまたはTallyで提案を作成することができます。&#x20;

SnapshotやTallyのプロポーザルは、必ずしも元のeIP作成者が投稿する必要はなく、EULの最低基準値を満たさない場合には、他の人や代表者が投稿することも可能です。スナップショットまたは集計上の提案には、常にeIPへのリンクが添付されている必要があります。投票のパラメータ(Yes, No, 値の異なる選択肢)は、eIPで議論された選択肢を反映させる必要があります。&#x20;

無効または不十分なサポートにより却下された提案は、再提出をすることができる。ガバナンス/投票によって十分な支持を得た承認済みの提案は、Euler Foundationによって実施されます。
