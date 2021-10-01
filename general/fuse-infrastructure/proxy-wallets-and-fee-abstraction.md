# Proxy Wallets and Fee Abstraction

The two key features of the Fuse wallet technology are the use of proxy wallets and fee abstraction.

## Proxy wallets

All Fuse wallet accounts are created in the form of proxy wallets. This means that each wallet is a smart contract on Fuse and the wallet owner is also the owner of the wallet smart contract. Only the wallet owner can initiate the actions made by the smart contract by signing transactions. 

The rationale for using smart contracts for wallet accounts is to enable new functionalities that are impossible or difficult to implement in the context of more traditional wallets that are just attached to the user's public address or addresses.

For instance, smart contracts can enable things like payment automation, regular payments and social recovery of the wallet in the case of access loss.

## Fee abstraction  

Fuse wallets also enable \(optional\) fee abstraction. If a wallet implements fee abstraction, for all or part of the transactions, the user will not have to pay network transaction fees on Fuse when making transactions. Instead, fee payments can be made on behalf of the users by any third party wishing to cover them.

At bottom, fee abstraction is achieved by separating the signature from submitting transactions to the blockchain. A Fuse wallet user still signs every transaction using their private key stored on their mobile phone. However, fee-abstracted transactions are actually submitted to the blockchain and paid for by the relevant relay service. 

The use of the proxy wallet approach makes it possible for the creator of a particular implementation \(fork\) of Fuse Wallet to determine which \(if any\) transactions sent by users will be covered by a third party. For instance, if a festival organizer creates a mobile wallet for the festival attendees, it may decide that the users shall be exempt from transaction fees when making payments during the festival.

   

