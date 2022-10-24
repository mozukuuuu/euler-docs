# リスクファクター

### 概要

このページでは、ガバナンスによって決定された、Eulerの主なリスクパラメータの概要を説明します。すべてのパラメータは以下の表1に表示されています。&#x20;

表1｜Eulerの担保、借入、リザーブファクターのパラメータ設定値

| Token     | collateralFactor | borrowFactor | reserveFactor | borrowIsolated | crossBorrow | InterestRateModel | Uniswap V3 fee tier (%) |
| --------- | ---------------- | ------------ | ------------- | -------------- | ----------- | ----------------- | ----------------------- |
| WSTETH    | 0.85             | 0.89         | 0.1           | false          | true        | Mega              | 0.05                    |
| STETH     | 0.87             | 0.91         | 0.1           | false          | true        | Lido              | Chainlink               |
| FLX       | 0                | 2.5e-10      | 0.23          | true           | false       | Default           | 0.3                     |
| AAVE      | 0                | 0.28         | 0.23          | true           | false       | Default           | 0.3                     |
| ANT       | 0                | 0.28         | 0.23          | true           | false       | Default           | 1                       |
| APE       | 0                | 0.28         | 0.23          | true           | false       | Default           | 1                       |
| BABL      | 0                | 0.28         | 0.23          | true           | false       | Default           | 0.3                     |
| BADGER    | 0                | 0.28         | 0.23          | true           | false       | Default           | 0.3                     |
| BANK      | 0                | 0.28         | 0.23          | true           | false       | Default           | 0.3                     |
| BED       | 0                | 0.28         | 0.23          | true           | false       | Default           | 0.3                     |
| BRIGHT    | 0                | 0.28         | 0.23          | true           | false       | Default           | 0.3                     |
| CARD      | 0                | 0.28         | 0.23          | true           | false       | Default           | 0.3                     |
| CNV       | 0                | 0.28         | 0.23          | true           | false       | Default           | 1                       |
| CTX       | 0                | 0.28         | 0.23          | true           | false       | Default           | 1                       |
| DPI       | 0                | 0.28         | 0.23          | true           | false       | Default           | 0.3                     |
| DPX       | 0                | 0.28         | 0.23          | true           | false       | Default           | 1                       |
| DYDX      | 0                | 0.28         | 0.23          | true           | false       | Default           | 0.3                     |
| ETH2X-FLI | 0                | 0.28         | 0.23          | true           | false       | Default           | 0.3                     |
| EXRD      | 0                | 0.28         | 0.23          | true           | false       | Default           | 1                       |
| FLOAT     | 0                | 0.28         | 0.23          | true           | false       | Default           | 0.3                     |
| FNT       | 0                | 0.28         | 0.23          | true           | false       | Default           | 1                       |
| FPIS      | 0                | 0.28         | 0.23          | true           | false       | Default           | 1                       |
| FRAX      | 0                | 0.28         | 0.23          | true           | false       | Default           | 0.3                     |
| FTT       | 0                | 0.28         | 0.23          | true           | false       | Default           | 1                       |
| FXS       | 0                | 0.28         | 0.23          | true           | false       | Default           | 1                       |
| GAMMA     | 0                | 0.28         | 0.23          | true           | false       | Default           | 0.3                     |
| GFI       | 0                | 0.28         | 0.23          | true           | false       | Default           | 1                       |
| GRT       | 0                | 0.28         | 0.23          | true           | false       | Default           | 0.3                     |
| GTC       | 0                | 0.28         | 0.23          | true           | false       | Default           | 1                       |
| IDLE      | 0                | 0.28         | 0.23          | true           | false       | Default           | 0.3                     |
| ILV       | 0                | 0.28         | 0.23          | true           | false       | Default           | 1                       |
| IMX       | 0                | 0.28         | 0.23          | true           | false       | Default           | 0.3                     |
| INDEX     | 0                | 0.28         | 0.23          | true           | false       | Default           | 1                       |
| LDO       | 0                | 0.28         | 0.23          | true           | false       | Default           | 1                       |
| LOOKS     | 0                | 0.28         | 0.23          | true           | false       | Default           | 0.3                     |
| LRC       | 0                | 0.28         | 0.23          | true           | false       | Default           | 0.3                     |
| LUSD      | 0                | 0.28         | 0.23          | true           | false       | Default           | 0.3                     |
| LYXE      | 0                | 0.28         | 0.23          | true           | false       | Default           | 0.3                     |
| MIM       | 0                | 0.28         | 0.23          | true           | false       | Default           | 1                       |
| MPL       | 0                | 0.28         | 0.23          | true           | false       | Default           | 0.3                     |
| MTA       | 0                | 0.28         | 0.23          | true           | false       | Default           | 0.3                     |
| MVI       | 0                | 0.28         | 0.23          | true           | false       | Default           | 0.3                     |
| NMR       | 0                | 0.28         | 0.23          | true           | false       | Default           | 1                       |
| OGN       | 0                | 0.28         | 0.23          | true           | false       | Default           | 0.3                     |
| RAD       | 0                | 0.28         | 0.23          | true           | false       | Default           | 0.3                     |
| RAI       | 0                | 0.28         | 0.23          | true           | false       | Default           | 0.3                     |
| RENDOGE   | 0                | 0.28         | 0.23          | true           | false       | Default           | 0.3                     |
| REQ       | 0                | 0.28         | 0.23          | true           | false       | Default           | 0.3                     |
| RPL       | 0                | 0.28         | 0.23          | true           | false       | Default           | 0.3                     |
| SETH2     | 0                | 0.28         | 0.23          | true           | false       | Default           | 0.3                     |
| SNX       | 0                | 0.28         | 0.23          | true           | false       | Default           | 0.3                     |
| SOCKS     | 0                | 0.28         | 0.23          | true           | false       | Default           | 1                       |
| SOS       | 0                | 0.28         | 0.23          | true           | false       | Default           | 1                       |
| STG       | 0                | 0.28         | 0.23          | true           | false       | Default           | 0.3                     |
| TCR       | 0                | 0.28         | 0.23          | true           | false       | Default           | 0.3                     |
| TORN      | 0                | 0.28         | 0.23          | true           | false       | Default           | 1                       |
| TRDL      | 0                | 0.28         | 0.23          | true           | false       | Default           | 1                       |
| UBI       | 0                | 0.28         | 0.23          | true           | false       | Default           | 1                       |
| VEGA      | 0                | 0.28         | 0.23          | true           | false       | Default           | 0.3                     |
| WAMPL     | 0                | 0.28         | 0.23          | true           | false       | Default           | 0.3                     |
| WILD      | 0                | 0.28         | 0.23          | true           | false       | Default           | 0.3                     |
| WNXM      | 0                | 0.28         | 0.23          | true           | false       | Default           | 1                       |
| WOO       | 0                | 0.28         | 0.23          | true           | false       | Default           | 0.3                     |
| XMON      | 0                | 0.28         | 0.23          | true           | false       | Default           | 1                       |
| YFI       | 0                | 0.28         | 0.23          | true           | false       | Default           | 1                       |
| 1INCH     | 0                | 0.5          | 0.23          | true           | false       | Major             | 0.3                     |
| AGEUR     | 0                | 0.5          | 0.23          | false          | true        | Stable            | 0.05                    |
| CVX       | 0                | 0.5          | 0.23          | false          | true        | Major             | 1                       |
| PERP      | 0                | 0.5          | 0.23          | false          | true        | Major             | 0.3                     |
| RBN       | 0                | 0.5          | 0.23          | false          | true        | Major             | 1                       |
| SHIB      | 0                | 0.5          | 0.23          | false          | true        | Major             | 1                       |
| USDT      | 0                | 0.5          | 0.23          | false          | true        | Major             | 0.3                     |
| OSQTH     | 0                | 0.56         | 0.23          | false          | true        | Major             | 0.3                     |
| AXS       | 0                | 0.66         | 0.23          | false          | true        | Major             | 0.3                     |
| ENS       | 0                | 0.66         | 0.23          | false          | true        | Major             | 0.3                     |
| MATIC     | 0                | 0.66         | 0.23          | false          | true        | Major             | 0.3                     |
| MKR       | 0                | 0.66         | 0.23          | false          | true        | Major             | 0.3                     |
| LINK      | 0.3              | 0.76         | 0.23          | false          | true        | Major             | 0.3                     |
| UNI       | 0.3              | 0.76         | 0.23          | false          | true        | Major             | 0.3                     |
| DAI       | 0.85             | 0.88         | 0.23          | false          | true        | Stable            | 0.3                     |
| WBTC      | 0.88             | 0.91         | 0.23          | false          | true        | Mega              | 0.3                     |
| WETH      | 0.88             | 0.91         | 0.23          | false          | true        | Default           | Pegged                  |
| USDC      | 0.9              | 0.94         | 0.23          | false          | true        | Stable            | 0.3                     |

_注：貸与資産の担保係数と借用資産の借用係数を掛け合わせ、最終的な係数を算出します。_

例えば、1,000USD分のUSDCを貸した場合、最終係数0.648（0.90×0.72）に合わせてUNIを借りることができるのです。したがって、648USD分のUNIとなる。

あるいは，500 ドル相当の USDC と 500 ドル相当の WETH を貸すと，リスク調整後の担保価値は (500 x 0.90) + (500 x 0.88) = 890 ドルである．もしUNIを借りるとしたら、890 x 0.72 = 640.8 USD相当のUNIを借りることができる。

もしあなたがより少ないUNI、例えば500ドル相当を借りたとしても、閾値に達する前にリスク調整された担保に対して追加のUNIまたはLINKのようなCross層の資産を借りることができることに注意してください。 最後に、リスク要因のリストは定期的に更新されることにご注意ください。

トークン/マーケットがDApp上で有効化されているにもかかわらずリストされていない場合、後ほど更新されたリストをご確認ください。
