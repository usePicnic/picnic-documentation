# Basket NFT

## What is a Basket NFT?

Whenever you put any crypto assets into Picnic by creating or copying a portfolio, a new Basket NFT is minted. The Basket NFT owns all the funds deposited into it and its owner is the address that created it.

This Basket NFT has standard NFT functionalities: you can transfer it to someone else (all the assets in the portfolio will go with it), display it or list it for sale on OpenSea...

### Why a Basket NFT?

Building a portfolio produces a non-fungible result because every portfolio is slightly different as it depends on execution prices, different yields being generated over time according to deposit timestamps, etc.

## Wallet

Every Basket NFT owns a Wallet, which is a separate contract that owns all funds relative to that Basket NFT. Funds stored in a specific Wallet can only be accessed with explicit permission from the Basket NFT owner linked to that Wallet.

![An illustrated explanation of Picnic architecture. Note that there is one and only one Wallet for each Portfolio NFT](<../.gitbook/assets/User guide@2x (1).png>)

This architecture easily enables the Basket NFT to collect airdrops, yields in different and unexpected tokens and it is also more resistant to being hacked by other users, as Wallet funds can only be accessed with the explicit permission from the owner of the Basket NFT.

Different from other DeFI protocols which create a shared portfolio with **many** users, the portfolio funds in your own Wallet is **not shared between users**: this guarantees that **only** you (as the NFT owner) can decide what is the best allocation for your portfolio. For example, if there is 1.34253 ETH in your portfolio, you will keep exactly this amount in your portfolio until you, and only you, decide to allocate it differently.
