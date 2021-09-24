# Fuse Studio Overview

[Fuse Studio](https://studio.fuse.io) is the cornerstone of Fuse's mobile-centric infrastructure. It is a platform enabling businesses, organizations and projects to easily create and manage token-powered communities.

Currently, The Studio has three key components:

1\) **The Studio \(Playground\) Frontend**. This application enables the creation and management of simple token communities without writing a single line of code. It may, for instance, be used for demonstration or proof-of-concept purposes.

2\) **The Studio backend**. The Studio's backend consists of the factories for creating the smart contracts for each token community, the subgraph for The Studio, the Studio Server and IPFS node for storing the community data that is stored off-chain

3\) **The Studio API**.   

![Fuse Studio architecture](../../.gitbook/assets/image%20%283%29.png)

## Backend Infrastructure

The backend is composed of the following independent services

* Studio API Backend has two purposes. Provides an API for fast and convenient querying of the blockchain data for the Studio DApp. Transmits heavy and complicated transaction flows on behalf of the user.
* Fuse-funder service used to fund community members and wallet users on the Fuse blockchain.
* Fuse IPFS proxy used for fast fetching and storing data in IPFS.

## Studio Contracts

Fuse studio is designed to launch DeFi communities on the Fuse network. The community contract binds together most of the services and features of the Studio. Among other things it consists of:

* Entities List contract to store community members and their roles
* Community ERC20 tokens on Fuse network with transfer rules
* The community's ERC20 token \(if a community-specific token is used\). This is the token that the community creator issues as part of the community deployment process

## Plugins

The plugins are used to customize the community to your specific needs. These can be smart contracts, backend services or the integration of both. The currently available plugins are:

* Business List - allows you to add businesses to you community. Businesses are Entities List members with special roles.
* Join Bonus - define a join bonus for new community members.
* Fiat Ramp - Currently integrated to [Transak](https://transak.com/) and [Moonpay](https://www.moonpay.io/) to allow easy deposit and withdraw using Bank Accounts and Payment Cards.
* More plug-ins coming soon.

