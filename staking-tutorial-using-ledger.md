---
description: >-
  This tutorial will walk you through the steps on how to stake FUSE using
  Ledger hardware wallet and MyEtherWallet.
---

# Staking tutorial using Ledger

_This tutorial was made using Ledger Nano S with firmware version 1.6.1 and Ethereum app version on Ledger Nano S was 1.3.7._

**Step 1:** Please make sure that you have installed the latest version of Ethereum app on your Ledger as shown below.

![](.gitbook/assets/0%20%285%29.png)

**Step 2:** Go to [www.myetherwallet.com](http://www.myetherwallet.com/) and click **“Access my Wallet”**.

![](.gitbook/assets/1%20%288%29.png)

**Step 3:** Click “**Hardware**” then select “**Ledger**” then click “**Continue**” and then click **“Next”** as shown below.

![](.gitbook/assets/2%20%288%29.png)

![](.gitbook/assets/3%20%287%29.png)

**Step 4:** Once you click “Next” in the previous step now you will have to change the Network to **“Fuse network” and then** select the Wallet address you would like to Send/Receive FUSE tokens, accept the terms and conditions and click on **“Access my Wallet”.**

![](.gitbook/assets/4%20%288%29.png)

![](.gitbook/assets/5%20%285%29.png)

![](.gitbook/assets/6%20%286%29.png)

**Step 5:** Now that you have logged in to your address in Ledger through MyEtherWallet on Fuse network, you can see your Fuse address \(Fusenet\), balance, etc.

![](.gitbook/assets/7%20%284%29.png)

**Now let’s learn how to stake FUSE.**

**Step 6:** Click on **“Contract”** and then click on Interact with contract and

1. Enter the consensus contract address **0x3014ca10b91cb3D0AD85fEf7A3Cb95BCAc9c0f79**
2. Copy the consensus ABI from below link

[https://raw.githubusercontent.com/fuseio/fuse-network/master/abis/Consensus\_abi.json](https://raw.githubusercontent.com/fuseio/fuse-network/master/abis/Consensus_abi.json)

Click on **“Continue”**.

![](.gitbook/assets/8%20%282%29.jpeg)

**Step 7:**

From the drop down select the **“Delegate”** function and then copy the “**Validator address”** from the staking UI. Enter the amount of FUSE you want to stake under **“Value in ETH”** and click on **“Write”**. In the below example I have copied ”Liquify” validators address to stake.

![](.gitbook/assets/9%20%284%29.png)

![](.gitbook/assets/10%20%284%29.png)

Review and confirm the transaction on your Ledger. Once the transaction is confirmed on-chain it means you have staked your FUSE successfully.

Now lets learn to withdraw the staked FUSE.

**Step 8**: Follow Step 1 to Step 6 from above.

From the drop down select the **“Withdraw”** function and then copy the “**Validator address”** from the staking UI to which you have delegated your stake. Enter the amount of FUSE you want to stake under **“\_amount\(uint256\)”, “value in ETH”** should be 0 and click on **“Write”**.

![](.gitbook/assets/11.png)

Review and confirm the transaction on your Ledger. Once the transaction is confirmed on-chain it means you have unstaked your FUSE successfully.

