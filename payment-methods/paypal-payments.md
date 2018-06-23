# PayPal Payments

PayPal is one of the most widely used online payment methods. CloudWaitress makes use of PayPal's REST express checkout payment integration. This allows us to easily process payments on your behalf with the funds going straight to your account. Please be aware that PayPal is only available in certain countries and currencies. You can see them [here](https://developer.paypal.com/docs/integration/direct/rest-api-payment-country-currency-support/).

## **How PayPal Payments Work**

Once PayPal is enabled, the option will be available to customers during the checkout phase of their order. Upon selection, they can either login to their PayPal account, create an account or use their credit card and checkout as a guest in order to complete payment. When a PayPal order is placed, the payment is and only captured when an order status is updated to "Confirmed". Until the order is "Confirmed", the status of the payment will be pending.

![](https://downloads.intercomcdn.com/i/o/62039172/6edc1f562686de2150fac0f5/paypal-example.png)

## **Requirements**

In order to use PayPal with CloudWaitress, you will need a fully valid business account. If you already have a PayPal business account, you can skip this step. If you do not already have one, sign up at [https://www.paypal.com/au/webapps/mpp/account-selection](https://www.paypal.com/au/webapps/mpp/account-selection). You can also upgrade your personal account to a business one from within your account settings.

## **Connecting Your PayPal Account**

### **Create A REST API Application**

1. Head to the PayPal developer portal at [https://developer.paypal.com/developer/applications/](https://developer.paypal.com/developer/applications/) to create a REST application.
2. Log into your PayPal account using the login in button
3. Once logged in, scroll down until you see the title "REST API apps".
4. Press the "Create App" button.
5. Enter your business name for the app name, ignore the sandbox developer account field
6. Press the "Create App" button to complete this step.

![](https://downloads.intercomcdn.com/i/o/62039344/bb9e2ef6e1d9f7892ef73fcc/paypal-rest-api-create.png)

### **Copy Your LIVE Application Credentials To Use With CloudWaitress**

1. After creating your application, you will be on the page where you can copy your credentials.
2. Change from the "Sandbox" to "Live" view using the buttons on the top right to view your live application credentials
3. Scroll down till press "Show" below the "Secret"
4. You will now be able to see your "Client ID" and "Secret" keys
5. These are almost like a password, they can be accessed anytime by logging in here but make sure to never share them publicly as they enable control over your account
6. Copy both the full "Client ID" and "Secret" making sure to do so without copying any extra spaces or characters

![](https://downloads.intercomcdn.com/i/o/62039366/09e2a4ac6e047f31917c3a5f/paypal-rest-api-credentails.png)

### **Add Credentials To CloudWaitress**

1. Once you have those copied, go to your CloudWaitress dashboard payments settings page at "Basic Settings &gt; Payments" and select the "PayPal" tab
2. Paste the "Client ID" key into "Application Client ID \(Live\)" and the "Secret" key into "Application Secret \(Live\)"
3. Select the currency you want to accept PayPal payments in from the list
4. Save your settings to complete the setup process

![](https://downloads.intercomcdn.com/i/o/62039527/c64e8957bd70b5828c30dd76/paypal-add-details-to-cloudwaitress.png)

## **PayPal Fees**

Please be aware that using PayPal, like other online credit card processors, you will be charged a fee on every transaction. This has to be managed by yourself through your own PayPal account as we are not responsible for this. You can use the PayPal website to see the fees for your respective country and currency.

## **Refunds**

Currently, refunds must be manually processed from within your PayPal account. When a customer places an order using PayPal, once the order is "Confirmed" and the payment is captured, you will be able to see the transaction in your PayPal account and can manage it from there.

## **Disconnecting PayPal**

To remove PayPal as a payment option, simply remove your application Client ID and Secret from the CloudWaitress payment settings page.

