# Setting Up Order Printing

CloudWaitress allows you to manually and automatically print out new orders. This guide will show you how to set it up and troubleshoot issues. For more information on how printing works, see [https://www.cloudwaitress.com/support/features/printing](https://www.cloudwaitress.com/support/features/printing).

## **Requirements**

* Windows 7 / 8 / 10 either 32-bit or 64-bit
* A Windows-compatible printer with the drivers installed. Ideally a thermal receipt printer

Ensure you have met all the requirements before starting the setup.

## Setup Your Print Drivers + Paper Size

1. The first thing you need to do is make sure your printers drivers are installed on your PC. You can find drivers on your manufacturers' website
2. If your drivers are successfully installed, your printer will be shown on your PC under "Control Panel" - "Hardware and Sound" - "Devices and Printers"
3. To verify the printer is working fine, right click it, select "Printer Properties" and press "Print Test Page" on the bottom right. You can also try printing to it from other programs like your web browser to test it's working.
4. Under your "Printer Properties", select "Preferences" at the bottom and then select "Advanced" at the bottom again. There you will see your default paper size. See the image below for some help finding it. You need to set your paper size to one with the smallest possible height, ideally 210mm. Make sure to take note of the paper size as you will need it in the next step.

![](https://downloads.intercomcdn.com/i/o/61644155/caa1bf8834d399eee2d1aece/printer-paper-size.JPG)

## Create A Print Configuration

![](https://downloads.intercomcdn.com/i/o/61644157/01ba4e1877a7a8bd38b207c1/print-configuration.JPG)

1. Log in to your CloudWaitress account. Go to the "Advanced Settings &gt; Printing" page to create and edit your print configurations.
2. Start creating a new print configuration. Under "Print Settings", leave "Paper Height Modifier" blank and enter your printer paper height from the previous step into the "Paper Height" field.
3. You total paper width is equal to the "Paper Width" setting plus the "Paper Margin" setting for each side. That means if your printing on 80mm thermal rolls, you can set the paper width to 72mm and the margin to 4mm.
4. Read the the following article to learn what all the settings do in detail - [https://www.cloudwaitress.com/support/features/printing](https://www.cloudwaitress.com/support/features/printing).
5. After creating your print configuration, take note of your API key as you will need it for the next step.

## Configure PushPrinter

![](https://downloads.intercomcdn.com/i/o/61644159/9ade23646ed7511328959247/image.png)

1. Download and install PushPrinter from this link [https://rebrand.ly/95743](https://rebrand.ly/95743)
2. Download and install Ghostscript, a program used to print files on Windows. Take note of the folder you install it in. Download link - [http://rebrand.ly/dad27](http://rebrand.ly/dad27)
3. Open PushPrinter, enter your API key from the print configuration you created in the previous step.
4. Click the Ghostscript path field and the file select box will pop up. Navigate to the folder you installed Ghostscript in. There you will see a bin folder, inside there you will see a file called "gswin32c.exe" or "gswin64c.exe", select it
5. Select your printer from the dropdown list and add additional printers if required
6. Press "Start Service" to start the printing service

## Test Print

1. Visit your orders page and test print an order by selecting "Print" from the 3-dot action drop-down on the right. You can also print by clicking an order and selecting "Print Order" from the action drop-down at the top. If you enabled auto-print, try placing an order to test the auto-printing.
2. We recommend printing both short and long orders to ensure that there is nothing being cut out vertically.
3. If you are having issues, read the troubleshooting tips below to help solve any problems that you might be experiencing. Feel free to contact us to give you a hand calibrating your printing

## Calibration & Troubleshooting

### **Sides being cut-off**

Start by reducing either your margin or paper width values under your printer configuration in your admin dashboard. You will eventually calibrate a suitable width and margin. You can also adjust the font size to something smaller.

You can get your correct paper width under your Windows settings as seen in step 1 at the bottom.

### **Not Printing Correctly**

To get the ideal print results, you will need to do the following:

* Find your printers default paper height and width in your Windows settings. Refer to the image at the bottom of step 1 to see how to do this.
* Enter the correct paper settings in millimetres into your printer configuration settings. Ignore the "Paper Height Modifier" field.
* You will likely notice that large orders printed have a small gap between each page length when being printed on a thermal receipt printer. This is something that we unfortunately, cannot fix.

### **Invalid API Key**

The API key you entered does not below to any of your print configurations. Double check your API key

### **Could Not Authenticate**

Check your internet connection or try again shortly

### **Printing not working even though everything is set up correctly**

Please ensure that Windows detects your printer. Try restarting your printer or PC. Try printing to your printer from other programs on your PC such as your browser.

### **Printer not being detected in Windows**

You need to find the correct driver for your printer provided its available for Windows. Try googling your printer name followed by the words "windows {insert your windows version} driver"

### **Qty, item and price is appearing multiple times per receipt**

Set a longer default paper size on your Windows settings for your printer.

### **The end of the receipt doesn't come out fully**

Under your Windows printer settings. Set your "Feed Line After Printing" option to a high value to allow the printer to feed through a few extra lines.

### **Excess whitespace at the end of a receipt**

Thermal printers generally trim out any excess whitespace when printing. If this is happening to you, please contact us.

### **Nothing above is fixing the issue**

Please contact us and we will help you sort it out.

