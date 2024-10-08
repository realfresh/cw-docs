---
description: >-
  Enabling Facebook ordering will allow your customers to order from your
  Facebook page.
---

# Setup Facebook Ordering

{% hint style="danger" %}
As much as this feature sounds great, it's honestly not very pleasant for people to order through Facebook. These tabs are also only available in desktop versions of Facebook further limiting them. That means it won't work on for users on their mobile phones. Facebook also makes regular updates and sometimes things break unexpectedly. As such, overall we recommend against using this feature. Simply directing people to your ordering domain is a far more reliable option.
{% endhint %}

Visit [https://developers.facebook.com](https://developers.facebook.com). If you are not already signed into Facebook, you can sign in with your regular Facebook account.

Once done, select the "My Apps" button on the top right and select "create new app".

![](https://storage.crisp.chat/users/helpdesk/website/e903fdb8557a9800/image\_f92n5y.png)

Enter your business name for your app name along with your email address and press create

After creating the app, you will be taken to the app dashboard. On the left menu, go to "Settings > Basic"

![](https://storage.crisp.chat/users/helpdesk/website/e903fdb8557a9800/image\_wtsxiz.png)

Choose "Page Tab". You will now need to fill in your store URL under "Secure Page Tab URL" and what you want to call your page tab under "Page Tab Name". Your store URL can either be your CloudWaitress subdomain such as "[https://yourdomain.cloudwaitress.com](https://yourdomain.cloudwaitress.com)" or your custom domain name if setup

![](https://storage.crisp.chat/users/helpdesk/website/e903fdb8557a9800/image\_cb565a.png)

To add the page tab to your Facebook page, you will need your Facebook App ID which you will see highlighted in orange in the previous photo at the top of the page

Next, you need to visit the following URL into your browser making sure to replace  with your Facebook app ID and  with the store URL that you entered previously

[https://www.facebook.com/dialog/pagetab?app\_id=\{{YOUR\_APP\_ID\}}\&redirect\_uri=\{{YOUR\_STORE\_URL\}}](https://www.facebook.com/dialog/pagetab?app\_id=\{{YOUR\_APP\_ID\}}\&redirect\_uri=\{{YOUR\_STORE\_URL\}})

If done correctly, you will see a page on Facebook saying "Add Page Tab" and you will be able to select one of your Facebook pages

If done correctly, you will see a page on Facebook saying "Add Page Tab" and you will be able to select one of your Facebook pages
