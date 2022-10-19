# 転送(Transfer)

### About

転送は、ユーザーがEulerのサブアカウント間で預金および債務資産を移動させることを可能にします。ユーザーは、資産を移動する前に、借入ポジションが関連するサブアカウントに十分な担保資産を持っていることを確認する必要があります。

### Step-by-step

**Transfer ETokens**

1. Ensure that you have sufficient deposits in the sub-account you are transferring from.
2. Select the Euler sub-account that you want to transfer from.
3. Select the Euler sub-account that you want to transfer to.
4. Select the asset you are interested in.
5. Enter the amount you wish to transfer:
   * Select `Max` to transfer all the selected asset deposits (or maximum amount possible based on your 'from' sub-account positions).
   * Select `Safe Max` to transfer enough such that your 'from' Euler sub-account will result in having a health score of 1.25.

**Transfer DTokens**

1. Ensure that you have sufficient debt tokens in the sub-account you are transferring from.
2. Select the Euler sub-account that you want to transfer from.
3. Select the Euler sub-account that you want to transfer to.
4. Select the asset you are interested in.
5. Enter the amount you wish to transfer:
   * Select `Max` to transfer all the selected asset debt (or maximum amount possible based on your 'to' sub-account positions).
   * Select `Safe Max` to transfer enough such that your 'to' Euler sub-account will result in having a health score of 1.25 (not supported for self-collateralized loans).

### FAQ

**Can I transfer multiple assets?**\
\*\*\*\*Yes, you will need to make multiple actions sent to the transaction builder.
