---
description: How to guide to print with a network printer
---

# Printing - Windows Network Printing

## **Network printing**

1. Please go to the Windows Control Panel

![](../.gitbook/assets/untitled%20%281%29.png)

1. Open Devices and Printers

![](../.gitbook/assets/untitled-1.png)

1. Right click and select 'Printer Properties'

![](../.gitbook/assets/untitled-2%20%285%29.png)

1. If your printer is not showing use these instructions to set it up [Printer Set up](https://www.notion.so/cloudwaitresswiki/Printing-Add-a-printer-18689e4654fe4978b20aeb82b581d81e).
2. To test that the printer is working, please press Print Test Page

![](../.gitbook/assets/untitled-3%20%281%29.png)

1. If the test page does not print. Then please connect and install the printer correctly. Please see : [Printer Set up](https://www.notion.so/cloudwaitresswiki/Printing-Add-a-printer-18689e4654fe4978b20aeb82b581d81e).
2. Open the PushPrinter for Windows program application
3. Go to the 'settings' cog and select the default or CloudWaitress provider profile from the dropdown list.

![](../.gitbook/assets/untitled-4%20%282%29.png)

1. Enable 'Automatically start PushPrinter'. \(This allows the application to auto-start when resetting your machine\).

![](../.gitbook/assets/automatically-start-pushprinter.png)

1. Press the printer button

![](../.gitbook/assets/untitled-6.png)

1. Using the Create Printer button, create printer

![](../.gitbook/assets/untitled-7%20%284%29.png)

1. Add settings including API key from the printer just created.

{% hint style="info" %}
**For a network printer:**

* Name the printer. 
* Add API printer \(found in the store printer settings\), 
* Set number of copies 
* Add printer IP address and set port to 9100\).
{% endhint %}

![](../.gitbook/assets/untitled-8%20%283%29.png)

{% hint style="danger" %}
**NOTE:**

**Printer name** - This is the name that the printer will show inside of CloudWaitress.

**API Key** - This needs to be copied from the printer settings inside of CloudWaitress.

**Number of copies** - This will determine how many copies of the are printed.

**Printing type** - This needs to be set to Windows Shared Printer \(ESCPOS\) for this to work.

**Windows Share Printer Name** - This must match EXACTLY the shared printer name that was added before. You should avoid spaces and special characters.
{% endhint %}

1. Test print
2. Create printer
3. Go to your store and place a test order.

\*\*\*\*

