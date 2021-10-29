# Fees

Each transaction in Polygon has a **transaction fee** that will be paid to a miner for including your transaction on its blockchain.&#x20;

This transaction fee depends on the complexity of operation (measured in [**gas**](https://ethereum.org/en/developers/docs/gas/#what-is-gas)) and the **gas price** set up by the user: the greater the gas price, the higher the probability of the transaction be included faster on the blockchain.&#x20;

{% hint style="info" %}
Currently Polygon does not use [EIP-1559](https://ethereum.org/en/developers/docs/gas/#eip-1559), and the [minimum gas price](https://forum.matic.network/t/recommended-min-gas-price-setting/2531) is 30 gwei, or 30 x 10$${}^{-9}$$ MATIC. &#x20;
{% endhint %}

Note that every transaction requires at least 21,000 gas, regardless of the complexity of the operation. Consequently, producing these transactions manually on Metamask, besides time-consuming, costs 12,000 gas **for each transaction**. On the other hand, by using our contracts, you can batch several operations in a **single transaction **avoiding this costly overhead.&#x20;

IndexPool also has a 0.1% fee for each deposit (ETH or ERC20 token) on your Wallet, which will be used to support new features for IndexPool.

**Summary of fees**:

| Operation                        | Transaction fee | IndexPool fee |
| -------------------------------- | --------------- | ------------- |
| Deposit of ETH/ERC20 token       | _Variable_      | 0.01%         |
| Withdraw of ETH/ERC20 token      | _Variable_      | 0%            |
| Creating Wallet                  | _Variable_      | 0%            |
| Transfer Wallet ownership        | __              | 0%            |
| Interaction with other protocols | _Variable_      | 0%            |
