# Printing

CloudWaitress supports automated and manual printing of order receipts through our web interface. You are able to print to any printer that is installed and configured to a Windows PC \(7, 8, 10 / 32-bit or 64-bit\).

To learn how to set up printing and troubleshoot issues, see [https://www.cloudwaitress.com/support/guide/setting-up-order-printing](https://www.cloudwaitress.com/support/guide/setting-up-order-printing)

## **How Printing Works**

Printing in CloudWaitress is done through an external software known as PushPrinter. This software allows you to connect to our servers and receive print jobs to your locally connected printer.

For PushPrinter to work, you will need one of 2 things. First is a stable internet connection. Second, you need to ensure that your printer is compatible with your PC and has the relevant drivers for it.

## **Printing Configurations**

CloudWaitress allows you to create multiple printing configurations for different printers or different store locations. Each configuration has the following options:

**Name**

This is just the name used to refer to this configuration in the system. You can choose anything you like to help you remember what this configuration does.

**Locations**

This determines which locations this printing configuration will be used for. We recommend one location per config but you can add as many as you like.

**API Key**

This is your unique "password" that identifies your printer configuration to our server. Take note of this as you will need to enter your API key into PushPrinter later when setting it up.

**Auto Print Orders**

Toggling this means the system will attempt to automatically print new orders placed at your store. If the order cannot be printed for whatever reason, we will re-try to print it in the next few minutes.

**Auto Print Only If Location Open**

If auto-printing is enabled, enabling this option ensures that the system won't attempt automated print jobs while your store is closed. Useful if your printer is not always online to prevent failed print jobs.

**Print Fail Email**

If entered and an order fails to print out for any reason, you will receive an e-mail informing you of the failure.

**Paper Settings**

These settings are required for our servers to generate a receipt that matches your printer paper settings. If this is not correct, your receipts will not print out correctly.

* Paper Width - The width of your printing paper \(millimetres\)
* Paper Margin - The margin or border around your paper \(millimetres\)
* Height Modifier - Obselete
* Paper Height - The default paper height in your windows print settings
* Font Size - Determines the size of fonts on your printout \(pixels\)

E.g. If you are printing on 80mm thermal paper rolls, you can enter 72mm for paper width and 4mm for paper margin which adds up to a total of an 8mm margin for both sides.

**Printout Customization**

This allows you to remove various parts of the receipt from being printed. For example, disabling "Dishes" means that the items ordered will no longer be included on the receipt.

For example, use this to create receipts that might only have the dishes on it which is useful for the kitchen staff which don't need to see the customer details.

**Custom Header & Footer**

This allows you to add custom header and footer header text to the top and bottom of your receipt. For example, at the top, you can add your business number and details to make it a tax receipt. The bottom can have a thank you message with your latest promo code for customers.

**Disable Configuration**

Toggling this disables this printing configuration without deleting it.

Finding Your Default Printer Paper Settings

![](https://downloads.intercomcdn.com/i/o/61653683/1f591628ea598c0b3f30e1f8/printer-paper-size.JPG)

If you need help finding your default printer paper size, on your PC, open "Control Panel &gt; Hardware & Sound &gt; Devices & Printers". Right-click your printer and select printer properties. Then select "Preferences" at the bottom and finally select "Advanced" at the bottom again. There you will see your default paper size. See the image above for some help finding it.

## **Manual Printing**

You can manually print an order either from the order action button on the right side of each order row or under the order detail pop-up.

![](https://downloads.intercomcdn.com/i/o/61653708/66e5c5ac592df49261d471c4/printing-1.PNG)![](https://downloads.intercomcdn.com/i/o/61653749/953f9010fc3b8087d55391a2/printbutton-modal.JPG)

## **Automatic Printing**

Automatic printing allows orders to be printed out automatically when a customer places an order through your online store. If the system initiates an automated print and for whatever reason PushPrinter is unable to confirm it received the print job, the system will try again several times over the next few minutes. You can also setup automated print failure notification email's to alert you to any print jobs that failed to occur.

To prevent the system from attempting automated print jobs while your store is closed and the printer is disconnected, you can set the "Auto Print Only When Store Open" option under your printer settings when editing a location.

## **Printing FAQ**

**What is the cost of printing?**

PushPrinter is completely free and there is no extra cost to print out receipts using CloudWaitress

**Is there a limit to how many computers I can install the print application on**

You can install the print application on any number of computers and you can use any number of printers

**Is there a limit to how many times I can print?**

There is no limit to the number of print jobs you can process

**How long does it take to print?**

Manually print jobs complete within 5-10 seconds. Auto-printing on average takes about 10-15 seconds

**Supported Printers**

The print application works off the drivers you installed on your computer for your printer. This means that it should work for any printer that you can print to from standard programs like your web browser.

You can even use PushPrinter with PDF print drivers that allow you to save orders as PDF's to your computer automatically.

