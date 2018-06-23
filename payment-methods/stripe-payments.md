# Stripe Payments

You can accept credit cards online using [Stripe](https://stripe.com/). It is currently supported in numerous countries with a variety of currencies. If Stripe is not supported in your country you can apply to try [Stripe Atlas](https://www.stripe.com/atlas). If you do not use Stripe you can also use PayPal for online payments. Below is our simple guide on setting up Stripe and managing your account.

## **How Stripe Payments Work**

When Stripe is enabled, customers can choose from the online payment option when checking out. If a customer selects "Card \(Online\)", the credit card field will drop-down below.

![](https://downloads.intercomcdn.com/i/o/62038875/47d8a0f3b0ec72cacbb894bd/stripe-example.png)

### **Payments Processed On Order Confirmation**

After completing the form and placing an order, we will validate that the card is able to make payment. The customer will not be charged yet. Once the order status is changed to "Confirmed" in the system, we will process the charge and payment will be made. You will need to "Confirm" online orders within 7 days otherwise we will no longer be able to capture the payment.

Your customer's payments are processed directly through your Stripe account and are not related to us in any way.

## **Connecting Your Stripe Account**

Connecting your Stripe account is extremely simple. If you do not already have an account, visit their website to create one.

Connecting your account requires your Stripe "Publishable Key" and "Secret Key". Both of these will allow us to process the payments for you. You can find both these keys under the "API" page in your Stripe dashboard. Make sure to use the "Live" key for real payments.

![](https://downloads.intercomcdn.com/i/o/62038890/e946a1b546c57da2b28dcd30/stripe-api-key.png)

Once you have these keys, go to the "Basic Settings &gt; Payments" page under your admin dashboard and select the "Stripe" tab. Enter your keys into the respective fields and select your default Stripe currency.

When entering your Stripe details, you have the option to set your global stripe details or location specific details. This way each of your store locations can use their own Stripe account.

## **Validating Your Stripe Account**

To successfully process charges, you will need to ensure your Stripe account is fully valid. Please ensure that you have completed all the necessary requirements under the account checklist as outlined on Stripes [going live checklist](https://stripe.com/docs/checklist).

## **Test Payments**

Stripe provides you access to two sets of API keys. One for testing and one for real use. If you enter the test keys into your Stripe payment settings in the admin dashboard, your credit-card payment option will trigger the test mode payment popup as indicated with the "Test Mode" icon on the bottom edge of the screen. Here you can use any of Stripe's [test credit-cards](https://stripe.com/docs/testing#cards) to test out online payments without actually being charged.

## **Stripe Fee's**

We are not responsible for your Stripe account management or fees. Your Stripe account is simply linked to your CloudWaitress account to process charges on your behalf with the money going straight to your account. As such it is important you are aware of Stripe's payment processing fees. You can read more here [https://stripe.com/us/pricing](https://stripe.com/us/pricing). Please also take the time to read their FAQ and support to clear up any issues you may have.

**Stripe Currency Conversions**

Stripe enables you to accept different currencies online depending on the country you are in. If your Stripe currency is different from your store currency, we will convert the order amount to your Stripe default currency using real-time exchange rates for payment to be made.

## **Issuing Refunds**

Currently, to process refunds or issue charge backs, you will need to login to your Stripe account and do this manually. When customers place orders and pay online, you will see the payments under your Stripe account along with the total, customer name, number and email. You can easily issue refunds from here. Soon we will integrate this directly into the platform along with other Stripe features.

