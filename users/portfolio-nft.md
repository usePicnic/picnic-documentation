# Portfolio NFT

## What is a Portfolio NFT?

Whenever you put any crypto assets into IndexPool by creating or copying a portfolio protocol, a new Portfolio NFT is minted. The Portfolio NFT owns all the funds deposited into it and its owner is the address that created it.

This Portfolio NFT has standard NFT functionalities, you can transfer it to someone else \(all the assets in the portfolio will go with it\), display it or list it for sale on OpenSea...

### Why a portfolio NFT?

Building a portfolio produces a non-fungible result because every portfolio is slightly different as it depends on execution prices, different yields being generated over time according to deposit timestamps, etc.

## Wallet

Every Portfolio NFT owns a Wallet, which is a separate address \(one and only one for each NFT\) that owns all funds relative to that Portfolio NFT. Funds stored in a specific Wallet can only be accessed with explicit permission from the Portfolio NFT owner linked to that Wallet.

![One and only one Wallet for Portfolio NFT](../.gitbook/assets/image%20%285%29.png)

This architecture easily enables the Portfolio NFT to collect airdrops, yields in different and unexpected tokens and it is also more resistant to being hacked by other users, as Wallet funds can only be accessed with the explicit Portfolio NFT owner permission.

Different from other DeFI protocols which create a shared portfolio with **many** users, the portfolio funds in your own Wallet is **not shared between users**: this guarantees that **only** you \(as the NFT owner\) can decide what is the best allocation for your portfolio. For example, if there is 1.34253 ETH in your portfolio, you will keep exactly this amount in your portfolio until you, and only you, decide to allocate it differently.

