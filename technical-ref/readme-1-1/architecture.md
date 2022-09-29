---
description: A high-level overview of Picnic's architecture
---

# Architecture

`DeFiBasket` inherits from the [ERC721 contract](https://docs.openzeppelin.com/contracts/4.x/api/token/erc721). Each NFT minted by Picnic deploys a Wallet contract that is associated with this NFT and the owner of the NFT (i.e. the caller of the `createPortfolio`).

Only the NFT owner can use his Wallet contract to deposit or withdraw MATIC and ERC20-compliant tokens by using the Picnic (ex-DeFi Basket) contract functions `depositPortfolio`, `editPortfolio` and `withdrawPortfolio`.

The communication between the Wallet and other DeFi protocols is made through the Bridge contracts: the function `useBridges` of each Wallet contract executes batched delegate calls to Bridge functions, allowing great extensibility and composability with multiple protocols. At the same time, this sandboxed architecture increases the safety of our users.

{% hint style="info" %}
Only essential functions are allowed in the Bridges in order to avoid hacks when interacting with [proxy contracts](https://cmichel.io/replaying-ethereum-hacks-furucombo/).
{% endhint %}

![Picnic architecture](<../../.gitbook/assets/Protocol @2x.png>)

The Picnic protocol acts as a gatekeeper to only allow Portfolio NFT owners to interact with their respective Wallet contracts.
