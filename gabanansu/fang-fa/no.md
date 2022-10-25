# 代議員の議決権

{% hint style="warning" %}
ガバナンスについて発言したい場合は、自分自身またはコミュニティの誰かに投票権を委譲する必要があります。この操作を行わないと、投票権を持たないため、Snapshot（オフチェーン）やTally（オンチェーン）で提案を作成したり投票したりすることができなくなることを意味します。
{% endhint %}

### About

要約すると、代議員とは、1回限りの設定作業（トークンのdelegate機能を実行して他のユーザーまたはトークン保持者自身に委任し、ガバナ契約による投票権の決定を可能にする）を完了したトークン保持者のことを指します。デリゲートになると、アクティブなプロポーザルに投票したり、十分な議決権を持っていればプロポーザルを作成したりすることができるようになります。プロポーザルに直接投票しない場合は、自分の投票権をデリゲートに渡すこともできます。 以下の委任のセクションでは、EULトークンのスマートコントラクトを使用し、Tally Governance Dashboardを介して委任することを説明します。 送信者から委任者に投票を委任する。ユーザーは一度に1つのアドレスに委任することができ、委任者の票数に加算される票数は、ユーザーのアカウントにあるEULの残高と同等です。投票は、現在のブロックから、送信者が再び委任するか、EULを譲渡するまで、委任されます。委任は、後述のスマートコントラクト機能、またはタリーのユーザーインターフェースから行うことができます。

### Step-by-step

Voting power delegation can be done via Etherscan, Tally (On-Chain) Governance dashboard or programmatically.

#### Etherscan

1\. Visit the [EUL token page](https://etherscan.io/address/0xd9fcd98c322942075a5c3860693e9f4f03aae07b) on Etherscan (shown below).

2\. Click on `Contract` (shown below) to view the EUL token smart contract code and interact with the contract via etherscan.

3\. Click on `Write Contract` (shown below).

4\. Click `Connect to Web3` to connect your Metamask wallet which will be used to confirm the delegate transaction. Once connected, you should see your wallet connect on etherscan as shown below.

5\. Click on `3. delegate` to expand the delegatee address input text field.

6\. Enter the address you wish to delegate your voting power to. This can be your wallet address if you are self-delegating or another wallet address (i.e., a community member or one of the active delegates on the [delegates list](https://app.euler.finance/delegates).

7\. Click on the blue `Write` button directly under the delegatee address text field.

8\. Finally, regardless of whether you are delegating to yourself or delegating to a delegate, you will be required to confirm the transaction in your Metamask wallet and this transaction will cost gas.

To check the address you are currently delegated to, you can click on the `Read Contract` tab next to the `Write Contract` tab and you will be presented with the window below.

Click on `10. delegates` (shown below) and paste your address in the text field and click on `Query` and it should show the address you have set as a delegate. If it shows the zero address, (i.e., 0x0000000000000000000000000000000000000000) then it implies you have not delegated to your wallet or to another address.

You can also check your current voting power.

To do this, click on `14. getVotes` (shown below) and paste your address in the text field and click on `Query`. If you have self-delegated, your voting power should be equal to the number of tokens you hold. If you have not self-delegated, or if you have delegated to another address, the query will return zero voting power.

#### Tally (On-Chain) Governance Dashboard

1\. Visit the [Euler on-chain governance dashboard](https://www.tally.xyz/governance/eip155:1:0xd8E2114f6bCbaee83CDEB1bD6650a28BBcF144D5) on Tally and connect your wallet where you hold EUL tokens.

2\. Click on `Delegate vote` at the top right corner of the screen.

3\. A pop-up window will appear with two options as shown below, i.e., Delegate to self or Delegate to an address. You can then choose on of these options from the pop up window, either to delegate to yourself or to another wallet address (i.e., a community member or one of the active delegates on the [delegates list](https://app.euler.finance/delegates)). By delegating to self, you retain your voting power. Next time there is an active proposal, you can choose to vote in any way you choose.

If you choose to delegate to an address or delegate, the following screen will be shown instead where you can enter the address you wish to delegate your voting power to.

This will not transfer any of your EUL tokens to the delegate, but rather only delegate all your voting power, i.e., you will be voting via a delegate or proxy who will be voting on your behalf or representing you at the polls!

You can always change the delegate later on or delegate to yourself again. This helps to ensure that there is a good degree of participation from the community on on-chain governance proposals voting.

4\. Finally, regardless of whether you are delegating to yourself or delegating to a delegate, you will be required to confirm the transaction in your Metamask wallet and this transaction will cost gas.

To recap, delegates are token holders that have completed a one-time setup process. Once you become a delegate, you can then vote on active proposals, and create proposals if you have enough voting power. If you choose not to directly vote on proposals, you can pass your voting power on to a delegate as we have seen.



#### Programmatically

For developers who wish to interact with the EUL token smart contract directly, the EUL contract has a delegate function defined with examples on how to interact with it shown below.

```
function delegate(address delegatee)
```

* `delegatee`: The address the sender wishes to delegate their votes to.
* `msg.sender`: The address of the EUL token holder that is attempting to delegate their votes.
* `RETURN`: No return.

**Solidity**

```
EUL eul = EUL(0x123...); // contract address
eul.delegate(delegateeAddress);
```

**Web3.js**

```
const tx = await eul.methods.delegate(delegateeAddress).send({ from: sender });
```
