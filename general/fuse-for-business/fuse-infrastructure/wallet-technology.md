# Fuse Wallet Technology



The Fuse white-label wallet (Fuse Wallet) is a cross platform (for iOS and Android) mobile crypto wallet written in Dart and built on [Flutter](http://https/flutter.dev/). It is running on top of the Fuse network, but can be plugged into any EVM compatible blockchain.

It can be freely forked by anyone wishing to create a customized version for their own purposes. The Fuse Wallet codebase is available [here](https://github.com/fuseio/fuse-wallet).

A standard implementation of Fuse Wallet is also available on both Android and iOS for those who wish to get familiar with how the basic app works and (or) quickly onboard users to a community created using the Fuse Studio [web interface](https://studio.fuse.io).

## How Fuse Wallet Works and Its Benefits  &#x20;

The user stores his wallet in the operating system secured storage. Transactions are signed with the private key which is encrypted locally on the device by the user. All the data is controlled by the user and shared on demand with 3rd party services using web3.0 interfaces. Private user data is also stored in a decentralized manner on 3box and IPFS in order to be able to share it or restore it. Fuse wallets are meant to be used with the Fuse Studio and can integrate any ERC-20 token by changing the default contract address.

Benefits of Fuse wallets:

* **Cost reduction** - Build your app once and use it on any  mobile and web platform
* **Fee abstraction** - Your users will never need to buy ETH to start using your service
* **Flexible** - Supports any ERC-20-compatible token, and is made to work with Fuse Studio contracts&#x20;
* **Non custodial** - Provide services without the liability of holding consumer funds
* **Advanced privacy**  -  User owned data and shared by the users with 3rd party services
* **Localized** - Available in several languages, help us with the translation [here](https://lokalise.co/public/783082135d36f14996c804.53212944/)
* **Web3.0 enabled** - Let your users access any dapp with no friction import and share their identity with 3rd parties

The two core features of Fuse wallets are **the use of the proxy wallet model and fee abstraction**.
