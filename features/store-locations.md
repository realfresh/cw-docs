# Store Locations

A location in CloudWaitress refers to a store location. All your basic restaurant settings and menus apply to all of the locations you create. You can create and edit locations under the "Locations" menu in the admin dashboard

![](https://downloads.intercomcdn.com/i/o/61647976/7d859601b9d6f3679746f26f/locations.png)

## **How Locations Work**

### **Single Location Store**

When customers order online, they will not be prompted to select a location. Delivery orders will also be validated against that single location.

### **Multi Location Restaurant**

When a customer orders online, if they select pickup, they will get to choose their store of choice. If they choose delivery, we will calculate which store is the closest to them and route the order to that location.

**Open & Close Location Status**

Every location can be opened and closed. An open location allows orders to be placed for the order time "Now". If the store is closed, orders can only be placed at a later time within your opening hours. If your restaurant is set to closed during one of your opening hours, then we will assume it's closed and will not allow customers to place orders for that time slot. The feature is here to ensure customers don't place orders when the store is not operational. You can also open or close a location using the actions menu \(3 dots\) on the side of a location row.

You can automatically open and close according to your opening hours by toggling the "Auto Open and Close" option under a locations settings.

If you have different pickup and delivery opening hours, enabling the option under a locations settings will allow you to define separate opening hours.

## **Location Settings**

### General

**Address**

The address of your store location. Our system uses google maps to verify addresses, calculate distances and driving times.

**Phone**

Your store contact number, shown to the customer and used purely for display purposes

**Map Zoom Level**

This will modify how zoomed in your google maps embed will be on your online store page for this location. Set this to a level where customers can easily identify where your store location is relative to everything else.

**Opening Hours**

Opening times are very important. They are shown on your store page alongside other location information. These are also used to determine when customers can place orders at a later time. As such it is very important that your opening times are correct. I.e. no overlapping or invalid times.

Opening times are highly customizable and each day can have multiple opening and closing time segments.

**Auto Open and Close**

To save you the trouble of manually opening and closing your store, you can toggle this option to make this automated. If you are open or closed at an unexpected time, manually disable this option and open or close your location as needed.

**Different Pickup & Delivery Times**

Allows you to enter sperate operating hours for pickups and deliveries.

### **Delivery Provider**

A delivery provider can be an external company that you use to do your deliveries or software you use internally to manage them. Right now we only support one integration for the [http://www.getswift.co](http://www.getswift.co/) delivery management platform software. You can use this software to manage your deliveries and provide real-time delivery tracking. Many delivery service providers also use this software to manage their fleet. If they do, you can connect to their account for them to manage your delivery orders.

**Integration**

Select your delivery software integration, more integrations coming in time.

**API Key**

Enter the API key to connect to your software to receive delivery quotes and book orders for delivery

**Auto Book Deliveries With Provider**

When enabled, deliveries will be automatically booked with your provider when an order is placed. Otherwise, you will need to manually book deliveries through the orders interface. If auto booking deliveries, we also recommend auto-confirming orders by enabling automated order statuses and setting the confirm order option to 0. The manual option is useful if you plan on doing some of the deliveries yourself.

**Override Delivery Provider Fee**

By default, your delivery provider will return a quote for the cost of the delivery which is then added to your customer's cart. Enabling this option will override the quoted fee with your own custom delivery fee which can be configured under your logistic settings.

