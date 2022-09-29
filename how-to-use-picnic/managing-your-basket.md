# 🧺 Managing your Basket

A list of all basket associated to your wallet address is available in the [My Basket](https://www.defibasket.org/my-portfolios) page. When selecting a basket, you'll access a dedicated page to that basket. There you'll be able to check detailed information and perform actions.

### Information&#x20;

![](<../.gitbook/assets/image (11) (1).png>)

List of information available on the basket details page:

* Portfolio Name, which can be changed as described below
* Overall Basket Value in US Dollars
* Estimated APY _(calculated proportionally to the asset allocation)_
* Amount of Rewards accrued until this date
* Investment performance graph, demonstrating total basket value variation in USD&#x20;
* Asset allocation table with details on the allocation amount for each asset, like:
  * Asset description and link to its contract address
  * Allocation amount in asset tokens and USD value
  * Protocols involved in that asset creation
  * Estimated APY for that asset
  * Rewards received for that asset until this date

### Basket Actions

Actions available to maintain or edit your basket:

#### **Renaming a basket**&#x20;

Just click on the pencil to the right of the portfolio name, then sign the message and wait for the name to be updated.

#### Claiming rewards

You may farm your rewards with a single transaction. After clicking on the `Claim` button, just choose between allocating rewards value according to the current basket allocation, or depositing the rewards in your basket in a token of your choice.

#### Depositing funds

This action allows you to increase the value of your basket by depositing additional funds. You will be asked for the amount and the input token in the usual deposit interface.

![](<../.gitbook/assets/image (13).png>)

Next, you will be able to select whether you want to Match portfolio allocation or not. If selected, the amount deposited will be invested following the basket's current asset allocation.

![](<../.gitbook/assets/image (16).png>)

#### **Editing** basket

When editing a basket, you're presented with the same interface used to create a new basket. On the left you have the list of assets to select. On the right you have the current selection or allocation.

**Include assets**: just select the box on the left of the desired asset. It will automatically populate the allocation list on the right with zero allocation percentage.

**Remove assets**: you click on the trash can icon on the Portfolio allocation area. It will eliminate the asset from the basket and free up the corresponding percentage.

**Replace assets**: the best way to replace assets of a basket is to remove the one you want to replace and then include the other. Currently there's no functionality to directly replace one for another.

> Important: we only allow basket edition if 100% of the funds are allocated on the selected assets. We included a calculator on the bottom part of the Portfolio allocation interface to assist in the calculation.

![Edit allocation interface](<../.gitbook/assets/image (9) (1).png>)

After you're done editing your allocation, you'll then be able to preview the transactions and the final allocation when clicking the `Next step` button.&#x20;

The final step after you've verified all the transactions and the final allocation is to click on the Edit button. This will trigger the transaction modal and the usual wallet approval flows.

#### **Withdraw** funds

When withdrawing your funds, you should perform the following actions:&#x20;

1. Click on the Withdraw button on the basket action menu on the left
2. Select the token you'd like to receive back your funds
3. Define the percentage of funds to be withdrawn.&#x20;

When selecting a percentage lower than 100%, Picnic you calculate the value to be withdrawn based on the overall basket value and the percentage input by the user. It will then make sure to keep the allocation percentages as they were before the withdraw event.&#x20;
