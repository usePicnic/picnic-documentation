# Risks

## Bridge risks

Only the Portfolio NFT owner can call bridges that affect its portfolio funds, so the only way a bridge can impact the funds is if the Portfolio NFT owner called them. Once bridges are called, they have complete control over wallet funds, so it is of utmost importance to only call bridges that are trusted.

Bridges that have not been reviewed by the DeFi Basket team are considered untrusted by DeFi Basket and will not be present by default in the UI. If you want to interact with untrusted bridges you may encounter malicious intent or unreviewed contracts that might be extra-risky.

{% hint style="info" %}
#### How to know if a Bridge was reviewed by DeFi Basket:

Only trusted and reviewed bridges are displayed by default in [defibasket.org](https://defibasket.org). We also have a [list of trusted bridges](https://docs.indexpool.org/developer/contracts/bridges/trusted-bridges). For maximum security, you can double check your transaction in our [transaction decoder](https://defibasket.github.io/checker/).
{% endhint %}

## Smart contract risks

DeFi Basket has been audited by [Certik](https://leaderboard.certik.io/projects/defi-basket). Moreover, all of DeFi Basket smart contract codes are available for public verification on [GitHub](https://github.com/defibasket/defibasket-contracts).&#x20;

**Note**: a successful audit is **not** a silver bullet. While it does significantly lessen the risk of a hack, it does not guarantee that our contracts or contracts that DeFi Basket integrates with (such as Aave, Autofarm, etc.) will avoid hacks.

## DeFi risk

Every action on a DeFi protocol carries all the risk embedded in that protocol, be it smart contract risk, risk of [liquidation at loss](https://youtu.be/aTp9er6S73M), or simply price risk. DeFi assets also have their own share of risks: some tokens can black-list addresses or even became undercollateralized, and as such, some tokens may lose value or even become worthless.

In order to mitigate this kind of risk, we are prioritizing integrations with protocols and tokens that have been battle tested, gone through audits, and that have significant value locked into them.
