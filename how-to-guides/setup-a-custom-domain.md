---
description: >-
  Learn how to connect your own custom domain name to your online store for
  better branding and SEO
---

# Setup A Custom Domain

## Setup Process

1. In the restaurant dashboard, see "Settings &gt; Website &gt; Domains &gt; Custom Domain"
2. Enter your domain name and press save
3. Go to your domain management panel where you registered your domain
4. Access your DNS records and add the DNS records listed below
5. After adding the DNS records, wait 10 minutes for it to take effect
6. Then press the "Generate SSL Certificate" button under your custom domain settings. 

If your DNS settings have taken effect, it will indicate the SSL certificate has generated successfully. Once generated, your site will be accessible on your custom domain name. If you are unable to generate the certificate, allow more time for your DNS settings to take effect.

## DNS Record To Add

| Record Type | Host | Value |
| :--- | :--- | :--- |
| A Record | www / order / anything | 35.238.2 .132 |

{% hint style="info" %}
The host value is the subdomain of your domain that your customer will need to visit to access the site. If the host value is "order" and your domain is "business.com", then your store URL will be "order.business.com"
{% endhint %}

{% hint style="warning" %}
**If you use "www" for your host value, then please add the following record as well**
{% endhint %}

| Record Type | Host | Value |
| :--- | :--- | :--- |
| A Record | @ / blank | 35.238.2 .132 |

Setting this will ensure if someone types in your root domain, i.e. example.com, they will be redirected to www.example.com

