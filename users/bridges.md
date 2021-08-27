---
description: WIP
---

# Bridges

## What are bridges?

Bridges are smart contracts that IndexPool uses to connect with other DeFi protocols.

For example we have a bridge to do swaps on Uniswap. It is just a wrapper that generates data in the format we need to process in back-end and display on the UI.

## How bridges interact with the Portfolio NFT?

Once a bridge is called it has the power to use available funds in the NFT. So it is extremely important only to interact with trusted bridges.

