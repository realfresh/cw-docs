---
description: >-
  Learn how to setup Stripe, our recommend online payments provider due to their
  streamlined setup and user experience
---

# Setup Stripe Payments

You can accept credit cards online using [Stripe](https://stripe.com/). It is currently supported in numerous countries with a variety of currencies. If Stripe is not supported in your country you can apply to try Stripe Atlas. Below is our simple guide on setting up Stripe and managing your account.

## How Stripe Payments Work

When Stripe is enabled, customers can choose from the online payment option when checking out. If a customer selects "Credit Card", the credit card field will drop-down below.

![Stripe payment example](https://storage.crisp.chat/users/helpdesk/website/e903fdb8557a9800/image_16wk7ks.png)

## Connecting Your Stripe Account

1. Create an account on the Stripe website if you do not already have one
2. Ensure you are viewing your live account and not your test account 
3. Login to your account dashboard. On the left navigation, go to "Developers &gt; API Keys"
4. Next, open up your restaurant dashboard and navigate to "Settings &gt; Payments &gt; Stripe"
5. Enable Stripe payments using the "Enable" switch
6. Copy the "Publishable Key" and "Secret Key" from the Stripe dashboard into the restaurant dashboard
7. Set your payment currency in the restaurant dashboard and save the settings

![Stripe API keys](https://storage.crisp.chat/users/helpdesk/website/e903fdb8557a9800/image_4cpfy8.png)

## Testing Payments

If you would like to do a test payment, copy your test API keys from Stripe. You can do this by toggling the "Viewing test data" switch.

![Stripe test data](https://storage.crisp.chat/users/helpdesk/website/e903fdb8557a9800/image_1bjx53a.png)

Once this is done, you can use the credit card number "4242 4242 4242 4242" with any valid expiry, CVC and zip code. This card will allow you to make a dummy payment.

## Validating Your Stripe Account

To withdraw online payments to your bank, you will need to ensure your Stripe account is fully valid. Pleae, ensure you have completed all their required validations.

## Stripe Fee's

We are not responsible for your Stripe account management or fees. Your Stripe account is simply linked to your CloudWaitress account to process charges on your behalf with the money going straight to your account.

As such it is important you are aware of Stripe's payment processing fees. You can read more here [https://stripe.com/pricing](https://stripe.com/pricing). Please also take the time to read their FAQ and support to clear up any issues you may have.

## Stripe Currency Conversions

Stripe enables you to accept different currencies online depending on the country you are in. If your Stripe currency is different from your store currency, we will convert the order amount to your Stripe default currency using real-time exchange rates for payment to be made.

## Issuing Refunds

Stripe refunds can be processed from your order management dashboard or the Stripe dashboard. In the order management dashboard, the refund payment option is available in the order details popup. Simply press the action select bar and choose "Refund Stripe Payment".

