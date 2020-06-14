# Studio overview

Fuse Studio is a DApp \(Decentralized App\) running on the Ethereum and Fuse networks.  It allows anybody with no technical knowledge to launch a community and integrate a token into it. With Fuse studio, a token is easily minted on Ethereum using a friendly wizard. And then moved trough the bridge to the Fuse-chain to add features to it and manage it.  
  
Via the DApp you can access to the contracts and the services of the Fuse network. You can launch your community on the Fuse network with a token bridged to Ethereum, intergate web3.0 services from the DeFi \(Decentralized Finance\) ecosystem. The community is upgraded by a variety of plugins that customize the community to your needs. It allows you to:

* Add to your community users, business, admins and more tailor made roles
* Define transfer and bonus rules for the community members
* Cover transaction cost for you customer
* Integrate a white label wallet
* Make bounties \(soon to come\)
* You can your own plugins \(soon to come\)
* Local dapp store \(soon to come\)

The logic is defined by Ethereum smart contracts compatible smart contracts and backend services that listen to the events on the blockchain. We prefer to use the Fuse chain for fast and cheap transactions, but some significant events are necessary to happen on the Ethereum network, as a gateway to the whole ecosystem. We do not own user private data, it is controlled by the user itself via 3box and stored in IPFS.

## Backend Infrastructure

The backend is composed of the following independent services

* Studio API Backend have two purposes. Provides an API for fast and convenient querying of the blockchain data for the Studio DApp. Transmits heavy and complicated transaction flows on behalf of the user.
* Fuse-funder service used to fund community members and wallet users on the Fuse blockchain.
* Fuse IPFS proxy used for fast fetching and storing data in IPFS.

## Contracts

Fuse studio is aimed to launch DeFi communities on Fuse network. The community contract binds together most of the services and features of the Studio. Among other things it consists of:

* Entities List contract to store community members and their roles
* Community ERC20 token on Fuse network with transfer rules
* ERC20 token on Ethereum. That's the token that the user issues part of the community deploy process
* [Multitoken bridge](https://github.com/fuseio/bridge-contracts) - to minimize friction and costs we extended the POA ERC20-ERC20 bridge contract to many-ERC20-to-many contract.

## Plugins

The plugins are used to customize the community to your special needs. They can be smart contracts, backend services or the integration of two. The available plugins now are:

* Business list - allows you to add businesses to you community. Businesses are entities list members with special role.
* Join bonus - new community members will receive a join bonus.
* Fiat Ramp - Currently integrated to [Transak ](https://transak.com/)and [Moonpay ](https://www.moonpay.io/)to allow deposit and withdraw using Bank accounts and payment cards.
* More plug-ins coming soon.



