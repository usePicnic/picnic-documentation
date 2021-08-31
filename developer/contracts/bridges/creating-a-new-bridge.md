---
description: WIP
---

# Creating a new Bridge



* When implementing a new bridge please make sure that these recommendations are followed before opening a PR to our repository:
  * The Wallet contracts always use `delegatecall` for calling the bridge's functions. Because of this, a in-depth review for [backdoors](https://underhanded.soliditylang.org/) and best security practices will be done for avoiding calls to ill-behaved and malicious contracts.
  * Take care when integrating with proxy contracts! A double `delegatecall` can [set up the address of the proxy contract implementation to a malicious contract](https://cmichel.io/replaying-ethereum-hacks-furucombo/).
  * Make sure that `address(this)` is used in the bridge code in order to use the address of the calling Wallet rather than using the bridge address
  * Check if functions of 3rd-party contracts revert before emitting an event in the bridge

