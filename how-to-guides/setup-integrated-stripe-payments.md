---
description: >-
  Learn how to setup Stripe+ payments.  This is our recommend solution for
  online payments due to their streamlined setup, user experience and self
  service options in our dashboard.
---

# Setup Integrated Stripe Payments

### Steps to Set Up Stripe+ Payments:

1. **Login:** Access your admin dashboard at [admin.cloudwaitress.com](https://admin.cloudwaitress.com).
2. **Navigate to Settings:** Go to **Settings > Payments > Add Payment Method > Stripe > Add Method**.

<figure><img src="../.gitbook/assets/Settings-payments-Stripe.png" alt=""><figcaption><p>Settings > Payments > Add Payment Method > Stripe > Add Method</p></figcaption></figure>

#### Recommended Minimum Settings for Stripe:

| Setting                        | Recommendation              | Notes                                                                                               |
| ------------------------------ | --------------------------- | --------------------------------------------------------------------------------------------------- |
| **Enabled**                    | On                          | Activates the feature                                                                               |
| **Stripe Secret Key**          | sk\_live                    |                                                                                                     |
| **Stripe Publishable Key**     | pk\_live                    |                                                                                                     |
| **Stripe Version**             | Version 2                   | Only use Version 1 if requested by CloudWaitress support                                            |
| **Currency**                   | AUD - Australian Dollar - $ | Use your local currency                                                                             |
| **Disable E-Mail Receipt**     |                             |                                                                                                     |
| **Enable Custom Payment Form** |                             |                                                                                                     |
| **Layout**                     | Themes                      |                                                                                                     |
| **Services**                   | Label                       | Pay - Online                                                                                        |
| **Delivery Label**             | Print Label                 | _PAID - ONLINE_                                                                                     |
| **Maximum Order Value ($)**    | 999                         | Set a realistic maximum online order total                                                          |
| **Minimum Order Value ($)**    | 2                           | Minimum transaction should not be lower than $2                                                     |
| **SC Account ID**              | GET THIS FROM SUPPORT       | Example format - acct\_1A3abABCABCac1aA. Contact chat/email support to activate your SC Account ID. |

3. **Save Settings:** Press **Save** to apply the settings.
4. **Test Your Setup:** Launch your store and place a live test order using your card, Google Pay, or Apple Pay.
5. **Get Assistance:** For any issues or to activate your SC Account ID, please email [support@cloudwaitress.com](mailto:support@cloudwaitress.com) or use the chat support feature.

### You can also activate the Stripe + Payments by connecting directly to Stripe

### Steps:

1. **Login:** Access your admin dashboard at [admin.cloudwaitress.com](https://admin.cloudwaitress.com).
2. **Navigate to Settings:** Go to **Settings > Payments > Add Payment Method > Stripe > Add Method**.
3. **Connect to Stripe:** Toggle to **Enable > Click Connect to Stripe .** This will route you to Stripe. Fill out the Stripe registration form and once complete, SC Account Id will automatically populate.&#x20;

<figure><img src="../.gitbook/assets/Screenshot 2025-03-18 at 10.39.20 AM.png" alt=""><figcaption></figcaption></figure>

4. Click  on Advanced Settings to complete the set up. Add sk\_live and pk\_live to the Stripe Secret Key and Stripe Publishable Key respectively > Save.

<figure><img src="../.gitbook/assets/Screenshot 2025-03-18 at 10.42.04 AM.png" alt=""><figcaption></figcaption></figure>



{% hint style="danger" %}
Please email [support@cloudwaitress.com](mailto:support@cloudwaitress.com) or use the chat support feature to get assistance activating this feature.
{% endhint %}

### Don't Have a CloudWaitress Account?

Visit [www.cloudwaitress.com](https://www.cloudwaitress.com) and click the **Sign Up** button on the top right to create your account.

{% content-ref url="using-stripe-integrated.md" %}
[using-stripe-integrated.md](using-stripe-integrated.md)
{% endcontent-ref %}
