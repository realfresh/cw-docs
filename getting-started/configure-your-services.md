---
description: >-
  Your restaurant services represent the various order types you accept. View
  our video for an in-depth explanation of all the settings available.
---

# Configure Your Services

{% embed url="https://youtu.be/EUW9nZVAE68" caption="Services video tutorial" %}

There are 4 services currently available. They are:

* Pickup - orders that are picked up in store by customers to take away
* Delivery - orders that are delivered to the customer's address
* Dine-in - orders that are placed by customers currently seated in your store
* Table booking - a reservation made for a later date and time

## How To Configure Your Services

1. Visit your restaurant dashboard and go to the settings page
2. Select the "Services" tab and edit your settings as required

## Enabling & Disabling Services

You can enable or disable services as needed. Go to the desired service settings and simply toggle the "Enabled" switch to enable or disable it.

{% hint style="info" %}
You must have at least one service enabled
{% endhint %}

## Service Notes

You can add custom notes for each service that will be shown to the customer when selected. Useful if you need to convey an important message to your customer

## Order Timings

A customer is only able to place an order due immediately if your store is opened. Orders for a later date must be scheduled within your opening hours. As such, order timings are mostly controlled by your store opening hours. From there, each service has it's own separate order timing settings that allow your more in-depth control.

### Enabling & Disabling Order Times

Under the "Order Timings" tab in the service settings, you can enable and disable both immediate and scheduled orders.

### First Order Offset

This is the period of time from when your store first opens to when you will accept the first order. For example, if the first order offset is set to 30 minutes and your store opens at 9:00am, the first order can be placed or scheduled at 9:30am.

### Last Order Offset

This is the period of time from when your store closes to when the last order will be accepted. For example, if the last order offset is set to 30 minutes and your store closes at 9:00pm, the last order can be placed or scheduled at 8:30pm.

### Order Offset

The normal order offset only applies for scheduled orders at a later time. This is the period from now when a scheduled order can be made. For example, it's there to prevent customers from scheduling order in the next 10 minutes instead of just asking for it to be due ASAP.

So for example, if your order offset is 30 minutes and the current time is 6:00pm, the next time a customer can schedule an order would be 7:00pm. If they want it before 7:00pm, they can still just order for ASAP instead. If the order offset was 15 minutes, then the customer can order for 6:30pm.

The order offset also acts as a cut-off point to give you time to meet the order schedule. For example, if it's 6:00pm and your order offset is 30 minutes. If the customer is scheduling an order for 7:00pm, they must place the order before 6:30pm. This is to give you 30 minutes to meet the scheduled time.

If they take too long and the time passes 6:30pm, they will receive a notification to tell them that the order has been changed to due ASAP instead of their scheduled time, 7:00pm.

## Custom Service Hours

Each service can have its own independent operating hours. Setting custom operating hours for a particular service will override the operating hours set for your store location.

## Estimated Wait Times & Auto Statuses

To help you better manage your orders and customer expectations, we provide a streamlined way to calculate order wait times and automatically update statuses. There are 6 order statuses:

* Un-confirmed
* Confirmed
* Ready
* On Route \(delivery only\)
* Complete
* Cancelled

Both wait times and automated status timings are connected to the timing settings. This is so that your status updates and wait times are in sync with each other. These timing settings are:

* **Time till confirm** - minutes between new **unconfirmed** to **confirmed** orders, use 0 for instant confirmation
* **Time till ready** - minutes between **confirmed** and **ready** orders. Effectively the time it takes you to prepare the food
* **Time till on route** - minutes between **ready** to **on route** orders. Effectively the time it takes for the food to be on the driver's vehicle and start delivery. This only applies to deliveries.
* **Time till complete** - minutes between the **ready** or **on route** to **complete** status. Useful for automatically marking orders as complete after a period of time.

\|\| The reason both wait times and automated status timings are connected to the same settings is so that your status updates and wait times are in sync with each other. If this was not the case, it would lead to customer confusion

### Automated Statuses

Automated statuses allow you to change an order's status after a set period of time has passed. This will allow you to do things such as:

* Automatically confirm new orders
* Mark orders as ready after a period of time
* Mark orders as complete after a period of time

This is very helpful if you know your business timings well and don't want to manually be updating order statuses.

Auto status updates can also be enabled or disabled on a per status basis. This way you can provide estimated wait times without auto-updating statuses. Or you can just instantly confirm orders and handle the rest manually.

For automated status updates to work, you will need to enable it for a particular status and ensure the timing settings are added to that particular status.

### Wait Times

Customer wait times are also calculated using the above timing settings. For pickup orders, the estimated wait time is calculating but adding the **time till confirm** with the **time till ready** values. So for example, if your **time till confirm** was 5 and your **time till ready** was 20. The customer would get an estimated wait time of 20 + 5 = 25 minutes.

For deliveries, the wait time is calculating by adding the **time till confirm** + **time till ready** + **time till on route** together. Then the **driving time** is added on as calculated using Google Maps. This provides the customer with an extremely accurate wait time for their order to be delivered.

