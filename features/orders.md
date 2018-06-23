# Orders

Orders are placed by your customers through your online store. They can also be placed through your mobile app if you enabled that feature.

Currently there is no way to manually enter orders through the admin interface. You can however do it manually through your own online store. Note that orders are seperate to table bookings.

## **Order Types**

There are 3 types of orders that you can accept.

* Pickups
* Deliveries
* Dine-in / Table side orders \(coming soon\)

You can configure settings for each of these order types through the "Settings &gt; Order Types" admin page.

### Pickups

These are orders that will be picked up in-person by your customer

**Pickup Notes**

These additional notes will be displayed under your store information, checkout and order confirmation if the order type matches this.

### **Deliveries**

Orders which will be delivered to the customer's desired location. There are several additional options you can configure to help you manage delivery orders.

#### **Delivery Notes**

These additional notes will be displayed under your store information, checkout and order confirmation if the order type matches this.

**Restrict Delivery Search Addresses**

This can be used to restrict all the delivery addreses show to the customer to a particular country. This allows local customers to find their address easier.

**Delivery Fee Type**

You can choose between 3 types of delivery fees. Leave the fee value field empty if you do not charge a delivery fee.

* Flat fixed fee
* Price per kilometer
* Kilometer fee brackets, e.g. between 0-5km / $5.00 and 5-10km / $10.00

**Free Delivery Amount**

Orders over this amount will receive free delivery. This does not include taxes or other fees and is based purely on the total value of the items added to a customers cart, not the final price.

**Minimum Order**

The minimum amount required for delivery orders. For example setting this to $20 means that customers have to order a minimum of $20 worth of food in order to check out. If empty there will be no minimum order for deliveries.

**Max Delivery Distance & Driving Time**

When a customer enter's their desired delivery address, we calculate the distance and driving time using google maps. A customer can only place an order if your store is within this delivery distance and driving time. Both are optional and if empty they will not be taken into consideration. It is recommended you at least set a max distance to prevent customers from placing orders that are far away and cannot be fulfilled.  
These additional notes will be displayed under your store information, checkout and order confirmation if the order type matches this.

## **Order Timings**

Orders can be accepted either now or later. You must enable at least one of these to accept orders. You can configure these settings through the "Settings &gt; Times" admin page.

### **Now**

Orders which are due immediately after being placed. Customers can only place orders of this type when your store is open. No additional options to configure

### **Later**

Orders which are pre-booked for a later time. Customers can place orders of this type within your designated locations opening hours. Please note that automated order statuses do not affect these orders. There are several options you can configure to manage these orders.

**Max Days Ahead**

This determines how many days ahead customers can place orders. Defaults to 7 if no value is entered.

**Time Interval**

The time interval in minutes between each order time slot. Defaults to 15 minutes of no value is entered

**Order Offset**

When placing an order, what is the minimum time in minutes from now that a customer can place an order. For example, if it is 7 pm and this is set to 30 minutes, customers can only place later orders from 7:30 pm onwards provided you are open. Defaults to 30 minutes if no value is entered. This is to prevent customers for placing orders for a later time when it should be placed for 'Now'

**First Order Offset**

If your opens at 8 am, setting this to 30 minutes means the first time slot available for customers to place orders will be 8:30 am. If empty this defaults to 30 minutes.

**Last Order Time**

Same as above but for closing times. If your store closes at 9 pm, setting this to 30 minutes means the last time slot available for customers to place orders will be 8:30 pm. If empty this defaults to 30 minutes.

## **Order Management**

We recommend that you read our detailed guide on how to receive and manage orders effectively. Find it at [https://www.cloudwaitress.com/support/guide/managing-orders](https://www.cloudwaitress.com/support/guide/managing-orders)

### **Order Statuses**

Order statuses are used to help you and customers manage and track your orders. There are currently 6 different order statuses

* Cancelled - orders which have been cancelled and will not be fulfilled
* Un-Confirmed - orders that have just been placed
* Confirmed - indicates that the order will be fulfilled
* Ready - the order is ready for collection or delivery
* On Route - if delivery, this indicates the order is on its way
* Complete - indicates that the order is complete including payment

You can see an orders status by its row color or pop-up header color. The color of the order will link to one of the corresponding statuses above.

![](https://downloads.intercomcdn.com/i/o/61647527/34c320b1dc6e1cff7f1dbbde/orders.png)

### **How Statuses Work?**

Statuses work in real-time on both your orders dashboard and on a customers order receipt. You can update statuses by press the 3 dots on the right of an order row or from within the order detail popup. The On-Route status is disabled for orders which are not deliveries. It is important to note that statuses work in a chain. I.e. unconfirmed orders can only be set to confirmed. Confirmed orders can only be set to ready. Orders can be cancelled at any time.

### **Automated Statuses**

To help you manage your order statuses, you can enable automated statuses under the "store &gt; status" menu link. This enables you to automatically change the status of orders based on how much time has passed from the point they were placed or their previous status. This feature only works for orders placed for 'Now', not 'Later'. Once you enable the setting, you will see 4 available options. Using them is simple. For example 'Time till Confirm' allows you to move an order from un-confirmed to confirmed. If set to 0, orders placed will automatically be set to confirmed. If set to 5, orders will be automatically updated to confirmed in 5 minutes unless manually updated to confirmed or above. Cancelled orders will not be affected at all.

These settings are extremely useful if you have setup your online store properly and you are aware of your business timings. For example if you know 99% of orders will be accepted and made within 20 minutes. You should set your 'Time till Confirm' to 0 and 'Time till ready' to 20. This way orders are updated automatically and can be manually changed if something changes

