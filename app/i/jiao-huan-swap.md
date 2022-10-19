# 交換(Swap)

### About

Eulerでの資産交換は、プラットフォームに統合された外部取引所（1inchまたはUniswap）を使用して、預けた資産を別の資産に交換することができます。

### Step-by-step

1. 交換したいアカウントに十分な供給資産があることを確認してください。
2. Select the Euler sub-account that you want to swap from.
3. Select the Euler sub-account that you want to swap to.
4. Select the asset you wish to sell.
5. Select the asset you wish to buy.
6. Enter the amount you wish to sell.
   * Select `Safe Max` to sell the amount such that your Euler sub-account will result in having a health score of 1.25.
   * Select `Liquidation` to sell the amount such that your Euler sub-account will end up at health score 1 (right on the edge of a liquidation).
   * Select `Max` to sell all the selected asset.
   * Users can set the `slippage` to the desired value by clicking the `gear icon` in the top-right corner.
7. Wait for a quote and click the `Swap` button.

### FAQ

**Can I swap assets from my wallet?**\
\*\*\*\*Currently, users can only swap assets they've deposited.
