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

Both estimated wait times and automated status updates are connected to the same timing settings. This is so that your status updates and wait times are in sync with each other. This avoids any customer confusion. These timing settings are:

| Setting \(minutes\) | From Status | To Status |
| :--- | :--- | :--- |
| Time till confirm | Unconfirmed | Confirmed |
| Time till ready | Confirmed | Ready |
| Time till on route \(delivery only\) | Ready | On Route |
| Time till complete | Ready | Complete |

{% hint style="info" %}
* Time till confirm is the time between when an order is placed to when it's confirmed. Setting time till confirm to "0" will result in instant order confirmation. You will need to also enable auto status for the confirmed status.
* Time till ready is the time it takes you to prepare an order after it's confirmed
* The time till on route status is effectively the time between when an order is prepared to when it is taken by the delivery driver.
* Time till complete is useful for automatically marking orders as complete
{% endhint %}

### Estimated Wait Times

A stated, customer wait times are calculated using the above timing settings. 

#### How estimated wait time are calculated for pickup or dine-in orders

For pickup and dine-in orders, the estimated wait time is calculating but adding the **time till confirm** with the **time till ready** values. So for example, if your **time till confirm** was 5 and your **time till ready** was 20. The customer would get an estimated wait time of 20 + 5 = 25 minutes.

If you have not added a value for time till confirm or time till ready, the estimated wait time would not be calculated.

#### How estimated wait time is calculate for delivery orders

For deliveries, the wait time is calculating by adding the **time till confirm** + **time till ready** + **time till on route** together. Then the **driving time** is added onto that. The driving time is determined using an external service that takes into account traffic data. This provides the customer with an extremely accurate wait time for their order to be delivered. Assuming 

If you have not added a value for time till confirm or time till ready or time till on route, the delivery time would not be calculated.

### Automated Statuses

Automated statuses change an order's status after a set period of time has passed. This will allow you to do things such as:

* Automatically confirm new orders
* Mark orders as ready after a period of time
* Mark orders as complete after a period of time

This is very helpful if you know your business timings well and don't want to manually be updating order statuses. Auto status updates can also be enabled or disabled on a per status basis. This way you can provide estimated wait times without auto-updating statuses. Or you can just instantly confirm orders and handle the rest manually.

For automated status updates to work, you will need to enable it for a particular status and ensure the timing settings are added to that particular status.

#### How automated statuses work

Status updates are dependent on your timing settings, the type of order and the order due time. It's best explained through a series of examples.

For the examples, we will assume our timing settings are as follows

* Time till confirm - 10 minutes
* Time till ready - 10 minutes
* Time till on route - 10 minutes
* Time till complete - 60 minutes

#### Pickup and dine-in examples

If a customer places an order at 7:00pm for pickup or dine in which is due immediately

| Time | Action |
| :--- | :--- |
| 7:00pm | Order has been placed, status unconfirmed |
| 7:10pm | Status updated to confirmed because time till confirm is 10 minutes |
| 7:20pm | Status updated to ready because time till ready is 10 minutes. This would also be the estimated order ready time as shown to the customer. |
| 8:20pm | Status updated to complete because time till complete is 60 minutes |

In the event that you added an extra 10 minutes onto the customers estimated order ready time, it will play out as follows:

| Time | Action |
| :--- | :--- |
| 7:00pm | Order has been placed, status unconfirmed, you add 10 minutes to estimated ready time |
| 7:10pm | Status updated to confirmed because time till confirm is 10 minutes |
| 7:30pm | Status updated to ready because the old ready time was 7:20pm, since you added an extra 10 minutes, that becomes 7:30pm |
| 8:30pm | Status updated to complete because time till complete is 60 minutes |

If we are unable to calculate an estimated ready time for the order, for example if the time till confirm was missing, it would play out as follows

| Time | Action |
| :--- | :--- |
| 7:00pm | Order has been placed, status unconfirmed |
| 7:05pm | You manually update the order status to confirmed |
| 7:15pm | Status updated to ready, because the time till ready is 10 minutes |
| 8:15pm | Status updated to complete because time till complete is 60 minutes |

If a customer places an order at 6:00pm for pickup or dine in which is due at 7:00pm, the following would occur

| Time | Action |
| :--- | :--- |
| 6:00pm | Order has been placed, status unconfirmed |
| 6:10pm | Status updated to confirmed because time till confirm is 10 minutes |
| 7:00pm | Status updated to ready, because this is when the customer scheduled the order for |
| 8:00pm | Status updated to complete because time till complete is 60 minutes |

#### Delivery examples

For the delivery examples, we will assume the driving time between your store and the delivery address is calculated as 10 minutes.

If a customer places a delivery order at 7:00pm which is due immediately

| Time | Action |
| :--- | :--- |
| 7:00pm | Order has been placed, status unconfirmed |
| 7:10pm | Status updated to confirmed because time till confirm is 10 minutes |
| 7:20pm | Status updated to ready because time till ready is 10 minutes |
| 7:30pm | Status updated to on route because time till on route is 10 minutes. This would also be shown to you as the driver pickup time |
| 7:40pm | Order will have been delivered to customer since the driving time is 10 minutes |
| 8:40pm | Order marked as completed because time till complete is 60 minutes |

If we were unable to calculate the estimated delivery time and driver pickup time, say if the time till on route was missing, the following would occur

| Time | Action |
| :--- | :--- |
| 7:00pm | Order has been placed, status unconfirmed |
| 7:10pm | Status updated to confirmed because time till confirm is 10 minutes |
| 7:20pm | Status updated to ready because time till ready is 10 minutes |
| 7:40pm | You manually mark the order an on route for delivery |
| 7:50pm | Order will have been delivered to customer since the driving time is 10 minutes |
| 8:50pm | Order marked as completed because time till complete is 60 minutes |

If a customer places a delivery order at 6:00pm which is due at 7:00pm, the following would occur

| Time | Action |
| :--- | :--- |
| 6:00pm | Order has been placed, status unconfirmed |
| 6:10pm | Status updated to confirmed because time till confirm is 10 minutes |
| 6:40pm | Status updated to ready because delivery time is 10 minutes and time till on route is 10 minutes, which means that the order must be ready by this time if it is going to reach your customer at 7:00pm |
| 6:50pm | Status updated to on route because the delivery time is 10 minutes, so it has to leave your store at this time. This is also the estimated driver pickup time. |
| 7:00pm | Order will have been delivered to customer |
| 8:00pm | Order marked as completed because time till complete is 60 minutes |

If a delivery order is scheduled for a later time but the estimated delivery time could not be calculated, then the ready and on route status will not update automatically.

{% hint style="info" %}
If ever in doubt about how the auto status timings will work for you scenario, just think about how it would logically work in a way that makes sense to your customer and you. That is how we have designed it to work.
{% endhint %}

