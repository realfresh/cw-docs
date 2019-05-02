# Setting Up a Custom Domain Name

## Already Have A Domain Name

### **Add DNS Record To Domain**

Simply login to your domain provider's admin dashboard and add the following DNS record to your domain.

* Type - CNAME
* Host - www / order / store \(pick any depending on where you want your site to be viewed on\)
* Value - stores.cloudwaitress.com
* TTL - Automatic

For example, if you use a host value of "order", then your online store will be located at "order.example-domain.com".

### **Send Us A Custom Domain Connection Request**

Navigate to the "Advanced Settings &gt; Domains" page in your admin dashboard and complete the custom domain request form. Once we process your domain within 24 hours, it will be activated.

## **Purchase & Setup A New Domain**

Purchasing and setting up your own domain is a very simple process that takes about 15 minutes. The below guide will help you do this with [https://www.namecheap.com/](https://www.namecheap.com/)

### **Purchase Your Domain Name**

1. Visit the Namecheap website at [https://www.namecheap.com](https://www.namecheap.com/)
2. Use the domain name search box at the centre of the page to look for a domain name
3. Add the domain name of your choice to your cart and then press the "View Cart" button on the right to progress through the checkout
4. Under your cart, we recommend disabling the "WhoisGuard" option that is enabled by default as this is not ideal for public businesses.
5. Select "Confirm Order" button on the right side and complete your order by creating an account and entering your payment details.

You can watch the following youtube video to see a video walkthrough of how to do this - [https://www.youtube.com/watch?v=Zbcn4skYXqM](https://www.youtube.com/watch?v=Zbcn4skYXqM)

### **Point Your Domain Name To Your Online Store**

Here you will need to modify something known as your domain name server \(DNS\) records. These are unique for every domain and determines what content your domain will display.

To modify your DNS records with NameCheap and point them to your online store, you will need to perform the steps below. If you are using a different domain provider, go to step 4 and add the required DNS records to your domain.

The following images were taken directly from NameCheap's article found here - [https://goo.gl/NFx37c](https://goo.gl/NFx37c)

\(1\) Visit [https://www.namecheap.com](https://www.namecheap.com/) and login to your account using the "Sign In" button on the top left

![](https://downloads.intercomcdn.com/i/o/62040312/ae00be5b0ff180102f273c65/sign_in.png)

\(2\) Once logged in, you will be re-directed to the admin dashboard at [https://ap.www.namecheap.com](https://ap.www.namecheap.com/). Select the "Domains List" on the left menu and then select the "Manage" button beside your domain name

![](https://downloads.intercomcdn.com/i/o/62040355/7173abfa04ca9bd998b8c1b2/domain_list_manage.png)

\(3\) Navigate to the Advanced DNS tab under your domain settings and select the "Add New Record" button

![](https://downloads.intercomcdn.com/i/o/62040430/5a3c3309e8cf0dd66e1c036c/advanced_new_record.png)

\(4\) Create a domain record with the following properties making sure to press the tick on the right to save the record

* Type - CNAME
* Host - www / order / store \(pick any depending on where you want your site to be viewed on\)
* Value - stores.cloudwaitress.com
* TTL - Automatic

\(5\) Optional - If you used "www" for the host value, create and save one more record. This says that if someone visits "[yourdomain.com](http://yourdomain.com/)" without the "www", redirect them to the "www" version.

* Type - URL Redirect Record
* Host - @
* Value - [https://www.\[yourdomainename\].\[extension\]](https://www.[yourdomainename].[extension]/)
* Value Type - Unmasked

Your records should look similar to below

![](https://downloads.intercomcdn.com/i/o/62040482/a3f0ccda2e10a0180e568251/namcheap-records.PNG)

### Submit A Custom Domain Request <a id="submit-a-custom-domain-request"></a>

The final step of the process requires a bit of work on our end

1. Login at [https://admin.cloudwaitress.com/](https://admin.cloudwaitress.com/) to your online store admin panel and using the main side menu, select "Settings &gt; Domains".
2. Under the "Custom Domain" section, enter your domain name, i.e. "[www.example.com](http://www.example.com/)" and press the button below to submit a request
3. We will review and process your request within 1-24 hours depending on how long it takes for your new DNS records to take effect.

Once we complete the setup process on our end, you will be notified. You can then find your online store by visiting your custom domain name.

