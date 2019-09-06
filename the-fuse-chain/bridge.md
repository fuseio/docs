# Bridge between Fuse chain & Ethereum

The bridge, based on POA's bridge implementation, is used to transfer Fuse tokens between the Fuse chain and the Ethereum network.

Tokens sent to the respective bridge contract on one network \(whether it's Fuse or Ethereum\) are "locked" in the bridge, "unlocked" on the other network bridge and transferred to the sender.

The validators of the bridge on both network are the Fuse chain validators. This means that validators, as part of their governance responsibilities, also need to validate bridge transactions and therefore hold Fuse tokens to "approve" bridge transactions on Fuse chain and hold ETH to "approve" transactions on Ethereum.

Each bridge transaction must be approved by a majority \(over 50%\) of the validators in order to be processed successfully.

The bridge contracts are deployed on both networks, and bridge oracle processes run on each validators machine as part of the validator deployment stack.

Besides the transfer of Fuse tokens between the two networks, the bridge is also responsible for network core functionality events:

**Mint block reward distributed on the Fuse chain on Ethereum**

Each cycle the total block reward distributed on Fuse chain is minted on Ethereum and locked on the bridge contract.

This works by listening to the \`RewardedOnCycle\` event emitted by the BlockReward contract on Fuse chain, waiting for all bridge validators on Fuse chain to sign it, and eventually sending a transaction to mint on Ethereum \(by the last signing validator\).

**Update Fuse chain validators on Ethereum**

Each cycle the Fuse chain validators are selected from a random snapshot of pending validators.

Those validators, being also the bridge validators, need to be updated on Ethereum as well.

This works by listening to the \`InitiateChange\` event emitted by the Consensus contract on Fuse chain, waiting for all bridge validators on Fuse chain to sign it, and eventually sending a transaction to set the bridge validators on Ethereum \(by the last signing validator\).

{% hint style="info" %}
Fuse chain bridge - [0xd617774b9708F79187Dc7F03D3Bdce0a623F6988](https://explorer.fusenet.io/address/0xd617774b9708f79187dc7f03d3bdce0a623f6988)

Ethereum bridge - [0x3014ca10b91cb3D0AD85fEf7A3Cb95BCAc9c0f79](https://etherscan.io/address/0x3014ca10b91cb3D0AD85fEf7A3Cb95BCAc9c0f79)

Fuse token on Ethereum - [0x970B9bB2C0444F5E81e9d0eFb84C8ccdcdcAf84d](https://etherscan.io/token/0x970B9bB2C0444F5E81e9d0eFb84C8ccdcdcAf84d)
{% endhint %}

