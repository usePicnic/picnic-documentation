# Bridge Helpers

Bridge helpers are contracts that help our current bridges to comply with more generic interfaces.

We currently have only one bridge helper, which is for the autofarm contract.

It exists because on the Autofarm contract, deposits require a poolId and the amount to be deposited. As poolId is something not standard and very specific to the Autofarm contract and there is no implemented method to easily get this info from the contract with an input address, we have implemented a contract that receives an ERC20 token address and returns a poolId.

This enables us to use the same interface for the Aave contract as well as for the Autofarm contract.

