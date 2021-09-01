---
description: A high level overview of IndexPool architecture
---

# Overview

IndexPool is an [ERC721-compliant contract](https://docs.openzeppelin.com/contracts/4.x/api/token/erc721): each NFT minted by IndexPool deploys a Wallet contract that  is associated to this NFT and the owner of the NFT \(i.e. the caller of the `createPortfolio`\).

The NFT owner can use his Wallets contracts to deposit or withdraw MATIC and ERC20-compliant tokens by using the IndexPool contract functions `depositPortfolio`, `editPortfolio` and `withdrawPortfolio`.

The communication between the Wallet and other DeFI protocols is made through the Bridge contracts: the function `useBridges` of each Wallet contract execute batched delegate calls to Bridge functions, allowing great extensibility and composability with multiple protocols.

![IndexPool architecture](../.gitbook/assets/indexpool-2x%20%282%29.png)

