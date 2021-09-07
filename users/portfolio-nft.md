# Portfolio NFT

## What is a portfolio NFT?

IndexPool is a DeFi portfolio sharing protocol, where you can copy, create and share portfolios with other people. Let's see how it works under the hood.

Those portfolios are represented by an NFT, which is a widely accepted standard for non-fungible assets, which are tokens that are differentiable from each other.

A portfolio NFT is basically a portfolio being represented by a token \(that can be transfered, displayed on opensea, or do anything else that can be done with an NFT\)

### Why a portfolio NFT?

Building a portfolio manually produces a non-fungible result because every portfolio is slightly different as it depends on execution prices, stake generating different yields over time depending on stake dates, etc.

As portfolios are non-fungible, using an NFT to represent them is the natural choice of architecture.

## NFT architecture

If you have 1.34253 ETH in your portfolio, you will be guaranteed to have exactly this amount in your portfolio, as it won't be shared in a Pool and exposed to some kind of rebalancing logic.

### Wallet

Each NFT owns a Wallet, which is a separate address \(one for each NFT\) that owns all funds relative to that NFT. This architecture also easily enables the NFT owner to collect airdrops, yields in different and unexpected tokens and also makes it much more robust in terms of funds being hacked by other users, as only NFT owner can access the Wallet funds.

![IndexPool contract relationship with Wallets](https://gblobscdn.gitbook.com/assets%2F-MbS412x4vAoAOC75BdK%2F-MiXSWGudfMI1r1XKgQ-%2F-MiXYxwH0kG4qdTlAcia%2FIndexPool%402x.png?alt=media&token=63dc3d4a-636c-4bf1-97c2-c550b456a487)

