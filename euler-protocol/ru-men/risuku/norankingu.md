# 資産のランキング

### 概要

各リスクパラメータは0（最高リスク）から1（最低リスク）まであります。リスクパラメータを組み合わせると、デジタル資産の総合指数となり、これも0から1までとなります。&#x20;

### **リスクパラメーター**

#### **スマートコントラクトリスク**

スマートコントラクトのリスクパラメータは、0、0.5、1のいずれかになります。 これは間違いなく最大のテールリスクです。スマートコントラクトの記述に不備があると、ハッキングや資金の盗難が発生し、価格の壊滅的な崩壊につながる可能性があるからです。 私たちは、プロトコルが監査されたかどうか、プロトコルがハッキングされずに機能している日数、必要であればより深い調査（ティアの昇格のため）などをチェックすることでこれを評価します。&#x20;

#### 集中化リスク

集中化パラメータは0から1まであります。 これは、少数の保有者がトークンに対して不当な影響力を持っているかどうかを測定するものです。例えば、トークノミクスのパイの70%を所有し、柔軟な権利確定期間を持つ創業者は、トークンを市場に過剰供給し、突然の売り抜けにつながる可能性があります。あるいは、トークンの大部分を保有するクジラが、ガバナンスを通じて容易に不利益な変更を行うことができます。 このリスクは、保有者ごとのトークン量の中央値を推定することで測定することができます。所有者構造が透明でない場合、フォレンジック・デューディリジェンスを採用します。&#x20;

#### ボラティリティリスク

ボラティリティのパラメータは0から1まであります。 他の条件がすべて同じであれば、実現ボラティリティが100%の資産は、実現ボラティリティが10%の資産よりも清算が発生しやすいと言えます。従って、ボラティリティの低い資産は、より有利な借入と担保の要因を持つはずです。 このパラメータは、担保のダウンサイドリスクと借入資産のアップサイドリスクに重点を置いて、実現ボラティリティ（および利用可能な場合はインプライド・ボラティリティ）を通じて測定することができる。&#x20;

#### 流動性リスク

流動性パラメータは0から1まであります。 他の条件がすべて同じであれば、1日の取引高が1億ドルの資産は、取引高が100万ドルの資産よりも売買がしやすくなります。 これは、借りたトークンを返済するために割引価格で担保資産を受け取る清算人にとって特に重要で、彼らは通常その担保をすぐに売るからです。もし彼らがその担保を売ることができず、または清算割引を与えられた適切な価格で借りた資産を買うことができなければ、彼らは清算をするインセンティブを持ちません。

これは不良債権の発生につながり、これを最小化する必要があります。 流動性の測定は、一定量のボリュームによって引き起こされる過去のスリッページを推定することによって行うことができます。 Uniswap v3上の既存のETH市場は、Euler上でアクティブになるための前提条件であり、私たちのオラクルはUniswap v3のTWAPに基づいているので、私たちはUniswap v3上のETHに対する流動性を推定していることに注意することが重要です。 つまり、あるトークンがUniswap v2上で非常に高い流動性を持っていたとしても、Uniswap v3上で流動性が低ければ、必ずしも高い借入係数を持つとは限らないということです。
