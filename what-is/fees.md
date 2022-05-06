# Fees

The only fee accrued by the DeFi Basket protocol is a **0.1% deposit fee**. All rebalancing that happens with already deposited funds is free from fees.

**Summary of fees**

Besides the DeFi Basket deposit fee, there are **protocol fees** and **transaction fees** that are explained in more detail further down the page.

#### Protocol Fees

Each protocol has its own fees, DEXes which are used for token swaps usually have fees in the range of 0.05% - 1%.

Protocol fees can be quite complex and we will dedicate more time in the future to break down how each of those fees work and give more transparency about that on our site.

#### Transaction Fees

Each transaction in Polygon has a **transaction fee** that will be paid to a miner for including your transaction on its blockchain.&#x20;

This transaction fee depends on the complexity of operation (measured in [**gas**](https://ethereum.org/en/developers/docs/gas/#what-is-gas)) and the **gas price** set up by the user: the greater the gas price, the higher the probability of the transaction being included faster on the blockchain.&#x20;

{% hint style="info" %}
Currently, Polygon does not use [EIP-1559](https://ethereum.org/en/developers/docs/gas/#eip-1559), and the [minimum gas price](https://forum.matic.network/t/recommended-min-gas-price-setting/2531) is 30 gwei, or 30 x 10$${}^{-9}$$ MATIC. &#x20;
{% endhint %}

Note that every transaction requires at least 21,000 gas, regardless of the complexity of the operation. Consequently, producing these transactions manually on Metamask, besides time-consuming, costs 12,000 gas **for each transaction**. On the other hand, by using our contracts, you can batch several operations in a **single transaction** avoiding this costly overhead.&#x20;
