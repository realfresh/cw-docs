# Customers Accounts



Customers include people who have placed an order at your online store or signed up for an account. From the restaurant perspective, it's about being able to track and understand your customers. For customers, having an account means their information is saved permanently across devices. This includes delivery details, customer info and past orders. This information will be used to pre-fill as many steps of their ordering process for a smoother repeat purchase experience.

## **Types Of Customers**

![](https://downloads.intercomcdn.com/i/o/61648903/0a8af242c3f15887024a6333/dashboard-example.JPG)

### **Guest Customers**

Guest customers are created whenever an order is placed by a user who has not signed in. We attempt to track guest customers by matching their name, phone and email address. When a guest places an order, if those 3 pieces of information match any past customers, the old customer will be updated instead of a new one being created.

Guest customer details are only saved temporarily on their device. We plan on adding an option to manually merge guest customers if you know they are indeed the same people who just used different information.

### **Logged In Customers**

A logged in customer is anyone who has used the login / sign up button to create an account. This button is only visible if you have at least one login method enabled \(more on this below\). When a customer signs up for the first time their details are logged into your customer dashboard. Any subsequent logins or orders will also update their details. Customers who log in will have their order history permanently accessible to them.

## **Login Methods**

![](https://downloads.intercomcdn.com/i/o/61648923/16fc3c7dc09ade4d564a0ae4/login-example.png)

Currently, we only support 2 login methods, Facebook & Google. The added benefit of social logins is that you can get other valuable customer data like gender, age, full name, profile picture, etc.

**Planned Upgrades**

* E-mail based logins
* Detailed customer reports
* Better customer management
* Customer promotion targeting
* Export customers to excel and CSV formats
* Fixing known issues listed below

**Caveats & Known Issues**

At the time of writing this, there are several known caveats and issues with customer logins that we will be addressing over time. These are:

* Facebook and Google logins can only be maintained for around 2-3 hours. After that time if a user is not active, they will need to re-login.
* Google web login cannot be used on a native mobile app as they have disabled it from being used in such a medium.

## **Setting Up Customer Accounts**

### Facebook

**Requirements**

* Facebook App ID
* Facebook App with the login addon and your domain whitelisted

**Steps**

1. Visit [https://developers.facebook.com](https://developers.facebook.com/) and login to your Facebook account
2. Select "My Apps" on the top right corner and then press "Add a New App"
3. Enter your restaurant name and contact email and press "Create App ID"
4. You will be taken to your app dashboard where you can add various Facebook products to your app. Hover over the "Facebook Login" addon and press "Set Up".
5. Select "Web" for the platform and enter your website URL, example "[https://demostore.cloudwaitress.com](https://demostore.cloudwaitress.com/)" and press save.
6. Copy your "App ID" as shown on the top left of the screen beside the nav bar.
7. Visit the customer's settings page in your dashboard at [https://admin.cloudwaitress.com/customers](https://admin.cloudwaitress.com/customers)and go to the settings tab. Enter your Facebook App ID and press save.
8. Visit your online store and test the Facebook login. Check your customer's page to see that the customer has been logged.

### Google <a id="google"></a>

**Requirements**

* Google Developer Account
* API access enabled and OAuth client ID

**Steps**

1. Visit [https://console.cloud.google.com](https://console.cloud.google.com/) and login to your Google Account
2. Accept the terms and conditions
3. Press "Select a project" on the top left. Then press the "+" button on the right side of the popup to create a project. Enter a project name and create it.
4. Wait for your project to be created, it might take some time. You can press "Select a project" again to see the creation status. Once created, select it if it's not already done for you.
5. Now open the left side menu and select "API's & Services" and then select "Credentials"
6. At the center of the screen, press the "Create credentials" button and select "OAuth Client ID" from the drop-down.
7. There will be a warning telling you "To create an OAuth client ID, you must first set a product name on the consent screen". Press the "Configure consent screen" button. Here you can enter your restaurant name, website URL and upload a logo. Once done press save.
8. You will be taken back to the credential creation process. Select "Web application" for the application type and enter any name for the key
9. For "Authorized JavaScript origins" and "Authorized redirect URIs", enter your full online store URL such as "[https://demostore.cloudwaitress.com](https://demostore.cloudwaitress.com/)".
10. Press save and you will be shown your client ID and secret keys. Copy the client ID as you will need to enter it into CloudWaitress.
11. Visit [https://admin.cloudwaitress.com/customers](https://admin.cloudwaitress.com/customers) and go to the settings tab. Enter your Google OAuth Client ID and press save.
12. Visit your online store and test the Google login. Check your customer's page to see that the customer has been logged.

### **Facebook Quickstart \(Not Recommended\)**

If you would like to enable Facebook customer accounts with minimal setup or just to test, you can use our CloudWaitress Facebook App ID.

We highly recommend you create your own accounts by following the Facebook steps below as this method has some limitations such as:

* Custom domain names cannot be used, you can only use a subdomain of CloudWaitress
* Your login process will not be white-labeled, customers will see that they are logging into the "CloudWaitress" platform.
* If you do decide to use your own Facebook ID at a later time, customers will no longer be matched to their existing accounts in your dashboard and instead, a new entry will be created for them. This means their previous order history will also be gone and all their analytics will reset.

**Quickstart Steps**

1. Visit [https://admin.cloudwaitress.com/customers](https://admin.cloudwaitress.com/customers) and login to your account
2. Select the "Settings" tab
3. Enter our Facebook App ID - 458001054545529
4. Save to enable customer accounts

