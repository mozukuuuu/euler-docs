# オラクルの評価

### オラクルとはなんですか**?**

価格設定の文脈では、オラクルは価格に関するオンチェーンAPIである。言い方を変えると、ある資産のある時点の価格を教えてくれるものです。

### オラクルのリスク

Uniswapのオラクルは私たちのパーミッションレスレンディングプロトコルに最も適していると考えていますが、Uniswap上の流動性の低い流動性プールに裏打ちされたEulerプールに預けると、壊滅的な結果につながることがあります。&#x20;

例えば、担保の価値を膨らませることで、攻撃者は膨れ上がった量のトークンを借りることができ、不良債権に繋がります。これは、レンディングプロトコルに対する最もシステマティックで広範な攻撃です。&#x20;

あるいは、借りた資産のUniswap V3オラクルが上向きに操作された場合、その攻撃はリクイデーションを引き起こし、借り手の担保を一掃する可能性があります。 さらに懸念されるのは、攻撃者が資産の価格設定をダウンサイドに操作できる場合です。仮に、価格がほぼゼロまで下落した場合、攻撃者はわずかな担保でプール全体を借り入れ、多額の利益を得て逃走することができます。

### オラクルリスク評価システム

オラクルの安全性を評価するために、我々のチームは与えられたUniswap v3 TWAPの移動コストを計算するツールを開発しました : [oracle.euler.finance](https://oracle.euler.finance/)

このツールを使って、TWAPを1ブロックと2ブロックにわたって上下に20.89%（最高品質の資産でブレークイーブンするために必要な最低値）動かす場合のコストを計算することができます。

<figure><img src="../../../.gitbook/assets/image (11).png" alt=""><figcaption></figcaption></figure>

そして、この4つの値の最小値である4億6,963万ドルを取り、以下の表に従ってレーティングを割り当てます。

<figure><img src="../../../.gitbook/assets/image (1).png" alt=""><figcaption></figcaption></figure>

その結果、UNI/WETHのプールの安全性は、1-2ブロックにわたる上下の攻撃コストが最低でも5000万円以上であることから、高いと判断された。

各レンディングプールのフロントエンドページに表示されます。

<figure><img src="../../../.gitbook/assets/image.png" alt=""><figcaption></figcaption></figure>

_**このツールはあくまでも指標であり、資金が失われた場合の責任は負いかねますのでご了承ください**_。

### オラクルの評価を上げるには**?**

もしあなたが、そのトークンのオラクルの評価を向上させ、より高い借入係数と担保係数を得ることを望むプロジェクトであれば、Uniswap V3でXYZ/WETHのペアにフルレンジの流動性を提供することが極めて重要です。

フルレンジの流動性とは、最低ティックから最高ティックまで、隙間なく流動性を提供することを意味します。

良い例は [METIS/WETH](https://info.uniswap.org/#/pools/0x1c98562a2fab5af19d8fb3291a36ac3c618835d9)

<figure><img src="../../../.gitbook/assets/image (10).png" alt=""><figcaption></figcaption></figure>

悪い例は [HEGIC/WETH](https://info.uniswap.org/#/pools/0xf2c3bd0328bdb6106d34a3bd0df0ef744551cc82), 流動性が超集中している。

<figure><img src="../../../.gitbook/assets/image (6).png" alt=""><figcaption></figcaption></figure>

より詳細な説明は、さまざまな操作のシナリオを紹介した[ビデオ](https://www.youtube.com/watch?v=snwUwj3QQ7M\&t=1s)をご覧ください。

ここで重要なのは、完全に普及した流動性が少量であっても、攻撃のコストを大幅に増加させることができる点です。例えば、[ IDLE/WETH](https://info.uniswap.org/#/pools/0x79e42a2bb91a0f9118e2b5231958c1eaefce390c) プールのTVLはわずか$52kですが、攻撃の最小コストはなんと$115millionになります。

<figure><img src="../../../.gitbook/assets/image (2).png" alt=""><figcaption></figcaption></figure>

### 参考文献

Darekが書いたオラクルツールの説明のブログ記事をご覧ください。[https://blog.euler.finance/uniswap-oracle-attack-simulator-42d18adf65af](https://blog.euler.finance/uniswap-oracle-attack-simulator-42d18adf65af)

フルレンジの流動性がわずかでもあれば、攻撃は信じられないほど高コストになってしまうという論文をチェックしてみてください。\
[https://github.com/euler-xyz/uni-v3-twap-manipulation/blob/master/cost-of-attack.pdf](https://github.com/euler-xyz/uni-v3-twap-manipulation/blob/master/cost-of-attack.pdf)
