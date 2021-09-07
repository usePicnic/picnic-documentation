---
description: A high-level overview of IndexPool architecture
---

# Architecture

IndexPool inherits from the [ERC721 contract](https://docs.openzeppelin.com/contracts/4.x/api/token/erc721). Each NFT minted by IndexPool deploys a Wallet contract that is associated to this NFT and the owner of the NFT \(i.e. the caller of the `createPortfolio`\).

Only the NFT owner can use his Wallet contract to deposit or withdraw MATIC and ERC20-compliant tokens by using the IndexPool contract functions `depositPortfolio`, `editPortfolio` and `withdrawPortfolio`.

The communication between the Wallet and other DeFi protocols is made through the Bridge contracts: the function `useBridges` of each Wallet contract execute batched delegate calls to Bridge functions, allowing great extensibility and composability with multiple protocols.

![IndexPool architecture](../.gitbook/assets/image%20%284%29.png)

The IndexPool protocol acts as a gatekeeper to only allow Portfolio NFT owners to interact with their respective Wallet contracts.

