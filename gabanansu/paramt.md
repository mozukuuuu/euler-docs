# パラメーター

### Introduction

このページでは、オンチェーンおよびオフチェーンのガバナンスパラメータについて概説します。

#### Tally (On-Chain) Governance Parameters

ここでは、Euler Governanceスマートコントラクト（[Tally](https://www.tally.xyz/governance/eip155:1:0xd8E2114f6bCbaee83CDEB1bD6650a28BBcF144D5)で管理）のガバナンスパラメータの概要を説明します。すべてのパラメータは、以下の表1に表示されています。 実行遅延、投票遅延、投票期間は、イーサリアムメインネットでのブロック作成時間を15秒と仮定したものです。 ガバナンススマートコントラクトは、OpenZeppelin  [GovernorSettings.sol module](https://github.com/OpenZeppelin/openzeppelin-contracts/blob/master/contracts/governance/extensions/GovernorSettings.sol) の機能を継承し、Voting Delay、Voting Period、Proposal Thresholdをオンチェーンガバナンス提案と投票プロセスを通じて更新することが可能です。

**Table 1** Euler オンチェーン ガバナンス パラメータ

| Parameter          | Value                   |
| ------------------ | ----------------------- |
| Voting Delay       | 11520 blocks (2 days)   |
| Voting Period      | 17280 blocks (3 days)   |
| Execution Delay    | 172800 seconds (2 days) |
| Quorum Numerator   | 3% of EUL Supply        |
| Proposal Threshold | 75,000 EUL              |

ガバナンスの提案が作成されると、2日間の審査期間（＝投票遅延）が設けられ、その後、投票の重みが記録され、投票が開始されます。 投票は3日間（＝投票期間）行われ、投票期間が終了した時点で定足数に達しており（十分な投票力がある）、賛成票が過半数を超えていれば、提案は成功したとみなされ、2日（48時間）後に実行することができます（＝実行ディレイ）。 75,000EUL以上の委任を受けたアドレスは、「提案のしきい値」を満たすことで、ガバナンス提案を作成することができます。 オンチェーンガバナンスのフェーズと各フェーズの期間は下図のとおりです。

#### Snapshot (Off-Chain) Governance Parameters

このセクションでは、オフチェーンガバナンス（[Snapshot](https://snapshot.org/#/eulerdao.eth/proposal/0x3b4b7e79c40df6860e7d612bdccc4969753e283dfd84673dc5fc4d201abcb317)で管理）のためのガバナンスパラメータの概要を説明します。すべてのパラメータは以下の表2に表示されています。

**Table 2** Euler オフチェーン ガバナンス パラメーター

| Parameter          | Value     |
| ------------------ | --------- |
| Voting Period      | 6 days    |
| Quorum             | 1,000 EUL |
| Proposal Threshold | 50 EUL    |

プロトコルのスマートコントラクトに直接的な影響がないため、オフチェーンガバナンスプロセスの投票遅延や実行遅延はありません。 50以上のEULを保有または委任されたアドレスは、提案しきい値を満たすことでガバナンス提案を作成することができます。議決権に関しては、委任された議決権またはプロポーザル作成ブロック番号のEUL残高が議決権にカウントされます。[Snapshot voting strategies](https://docs.snapshot.org/strategies/what-is-a-strategy) 投票方法は、`erc20-balance-of` と `erc20-votes`です。&#x20;
