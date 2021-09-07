# Risk

## Bridge risk

Only the Portfolio NFT owner can call bridges that affect its portfolio funds, so the only way a bridge can impact the funds is if the Portfolio NFT owner called them. Once bridges are called, they have complete control over wallet funds, so it is of utmost importance to only call bridges that are trusted.

Bridges that have not been reviewed by the IndexPool team are considered untrusted by IndexPool and will not be present by default in the UI. If you want to intereract with untrusted bridges you may encounter malicious intent or unreviewed contracts that might be extra-risky.

#### How to know if a Bridge was reviewed by IndexPool:

Only trusted and reviewed bridges are displayed by default in [indexpool.org](http://indexpool.org/). We also have a [list of trusted bridges](https://docs.indexpool.org/developer/contracts/bridges/trusted-bridges).

## Smart contract risk

IndexPool is currently on an unaudited version. Code is public on [github](https://github.com/indexpool/indexpool-contracts) and we expect an audit by Q4 2021.

## DeFi protocol risk

Every action on a DeFi protocol carries all the risk embeded in that protocol, be it smart contract risk, risk of liquidation at loss, or simply price risk.

In order to mitigate this kind of risk, we are prioritizing integrations with protocols that have been battle tested, gone through audits, and that have significant value locked into them.

