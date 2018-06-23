# Conditional Fees



Conditional fees allow you to add a charge to your customer's order based on certain conditions. You can use this to create credit card surcharges that add a 2.8% + $0.30 fee. Fees can be created under the "Store &gt; Conditional Fees" menu in the admin interface.

## **Fee Properties**

**Name**

Used to identify the fee and will be shown on the customer's receipt

**Fee Match Condition**

Determines under what conditions the fee will apply. If set to 'All', then all the conditions must be met before the fee applies. If 'Any', then if any condition matches, the fee will be applied. If the "All" option is selected, you will only be allowed to select one of each condition type.

**Fee Conditions**

These are the conditions upon which you can base your fees on. Currently, there are:

1. Order Timings - Now / Later
2. Order Logistics - Pickup / Delivery
3. Payment Methods - Cash / Card / Stripe / PayPal

**Fixed Value Fee**

Entering a value here will add a fixed fee to your customer's cart if the fee is applied

**Percent Based Fee**

If a value is entered, the respective percentage of your customer's cart total will be added on as a fee. This does not include other fees or costs. If both fixed and percent fees are provided, they will both be applied to the customer's cart.

Example - Credit Card Surcharge

To create a credit card surcharge of 2.8% + $0.30, you can do the following

1. Create a fee and enter 'Credit Card Surcharge' for the name
2. Select the "Any" match condition
3. Select both 'Stripe' & 'PayPal' from the payment method conditions
4. Enter '0.3' for the fixed fee and '2.8' for the percent fee
5. Save to complete and enable the fee

