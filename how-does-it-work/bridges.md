# Bridges

## What are bridges?

Bridges are smart contracts that Picnic uses to interact with other DeFi protocols. They are what enables us the possibility to integrate with any DeFi protocol, we just need to create a new bridge smart contract for a specific protocol and we are integrated to it.

To give you a sense of what functionality they accomplish, a bridge can execute swaps on Uniswap, perform deposits on Aave, or perform any arbitrary action with any other DeFi protocol. Bridges extend functionality into the Picnic protocol and emit events that are used to display transactions in the Picnic app.

## How do bridges interact with the Portfolio NFT?

![Wallets link with bridges to enable integrations with DeFi protocols](<../.gitbook/assets/Bridges @2x.png>)

Bridges are always called directly from the Wallet linked to the Portfolio NFT. Bridges have the power to use all the available funds in that particular Portfolio NFT. So, it is extremely important only to interact with trusted bridges (see below).

_See_ [_Picnic architecture_](../technical-ref/readme-1-1/architecture.md) _for a technical reference on how bridges interact with Picnic._

## What is a trusted bridge?

A trusted bridge is a bridge that was reviewed by the Picnic team. Once the Picnic protocol goes through an audit, trusted bridges will also be audited.

{% hint style="info" %}
Trusted bridges are the only available bridges by default in the Picnic app, which means that as long you as you don't add any custom bridges to your [usepicnic.com](https://usepicnic.com) app you are safe from interacting with untrusted bridges.
{% endhint %}

