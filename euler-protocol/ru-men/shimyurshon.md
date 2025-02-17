# シミュレーション環境

### 概要

不良債権を最小化し、かつ活動性を最大化するために、個々の資産と資産のポートフォリオについてテールリスクのシミュレーションを行い、ストレステストの清算シナリオを作成して、不良債権リスクを推定しています。&#x20;

### 例 1つの資産&#x20;

例えば、あるトークンが250位から30位に急上昇し、そのポジションを十分な時間維持できたことをインデックスリストで示した場合、異なる借入係数を与えて、貸付金全体に占める貸倒れの割合と活性度をシミュレートすることができます。その結果、借入係数を0.28から0.35に向上させることができます。&#x20;

### 例 資産のポートフォリオ&#x20;

あるいは、より複雑な環境で、低四分位値から50トークンを借り入れ資産として、高揮発性の状況で4つの担保資産（そのうち3つは時間が経過したもの、1つは新しい担保の提案）で一様に裏付けされたシミュレーションを行うことができます。テールリスクシナリオをシミュレーションすることで、プロトコルの最悪のシナリオを評価し、担保資産を含めることが適切であるかどうかを判断することができます。
