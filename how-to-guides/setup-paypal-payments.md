---
description: >-
  Learn how to accept online payments using your own PayPal account with our
  simple setup process
---

# Setup PayPal Payments

PayPal is one of the most widely used online payment methods. CloudWaitress makes use of PayPal's REST express checkout payment integration. This allows us to process payments on your behalf with the funds going straight to your account. Please be aware that PayPal is only available in certain countries and currencies. You can see them [here](https://developer.paypal.com/docs/integration/direct/rest-api-payment-country-currency-support/).

{% hint style="danger" %}
We highly recommend using Stripe instead of PayPal for online payments. PayPal occasionally has various service issues in our experience. See how Stripe payments guide instead below.
{% endhint %}

{% page-ref page="setup-stripe-payments.md" %}

## How PayPal Payments Work

Once PayPal is enabled, the option will be available to customers during the checkout phase of their order. Upon selection, they can either log in to their PayPal account, create an account or use their credit card and check out as a guest in order to complete payment.

## Requirements

In order to use PayPal with CloudWaitress, you will need a **fully valid business account**. If you already have a PayPal business account, you can skip this step.

If you do not already have one, sign up at [https://www.paypal.com/webapps/mpp/account-selection](https://www.paypal.com/webapps/mpp/account-selection). You can also upgrade your personal account to a business one from within your account settings.

## Connecting Your PayPal Account

### Create a REST API Application

1. Visit [https://developer.paypal.com/developer/applications/](https://developer.paypal.com/developer/applications/)
2. Log into your PayPal account using the login in button
3. Once logged in, scroll down until you see the title "REST API apps"
4. Press the "Create App" button
5. Enter your business name for the app name, ignore the sandbox developer account field
6. Press the "Create App" button to complete this step

![PayPal REST apps](https://storage.crisp.chat/users/helpdesk/website/e903fdb8557a9800/image_141scma.png)

### Copy Live Application Credentials

1. After creating your application, you will be on the page where you can copy your credentials
2. Change from the "Sandbox" to "Live" view using the buttons on the top right
3. Scroll down and press "Show" below the "Secret".
4. You will now be able to see your "Client ID" and "Secret" keys
5. In another window, go to your restaurant dashboard and to "Settings &gt; Payments &gt; PayPal"
6. Enable PayPal payments and paste in your "Client ID" and "Secret" key from the PayPal dashboard
7. Choose your payment currency and save the form

![PayPal application credentials](https://storage.crisp.chat/users/helpdesk/website/e903fdb8557a9800/image_1g9uc8i.png)

## PayPal's Fees

Please be aware that using PayPal, like other online credit card processors, you will be charged a fee on every transaction. This has to be managed by yourself through your own PayPal account as we are not responsible for this. You can use the PayPal website to see the fees for your respective country and currency.

## Refunds

Currently, refunds must be manually processed from within your PayPal account.

