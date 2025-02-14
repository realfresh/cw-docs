---
description: >-
  Learn how to setup and configure order printing for Android devices with our
  printing software
---

# Setup Printing For Android | CloudWaitress Printer Se

Our system allows restaurants to **automatically print order receipts** using an Android device. Follow this guide to set up and troubleshoot your **Android printer setup** for seamless printing.

{% hint style="info" %}
We are happy to remotely set up your printer for you. We know this is a step that can trip up many people due to every printer being a bit different. Please [contact us](https://www.cloudwaitress.com) via chat if you would like assistance.
{% endhint %}

### **Requirements**

Before you start, ensure you have:

* **An Android device** (running **Android 4.1 or later**)
* **A Bluetooth or network-connected ESC/POS printer**
* The **latest version of PushPrinter** ([_Download here_](https://pushprinter.com/))

## Setup Process

### Step 1: Create a Printer Configuration

1. Open your [**CloudWaitress dashboard**](https://admin.cloudwaitress.com).
2. Go to **Settings > Receipt Printing > Create Printer**.
3. Fill in:
   * **Printer Name -** i.e. "Android Kitchen Printer"
   * **Printing Method:** Set to _ESCPOS_
   * **Printing Type:** Use _ESCPOS Image_ for best results. (Note that some older printers may not support this method and ESCPOS Text Only can be used in these cases).
   * **Paper Scale Factor:** Adjust to **1.7** if text is cut off.
4. Click **"Save"** and copy your unique **API key** (needed later).

<figure><img src="../../.gitbook/assets/image (1) (2).png" alt=""><figcaption><p>Step 1, point 2</p></figcaption></figure>

![Printer Settings for Android](../../.gitbook/assets/printer-settings.png)

<figure><img src="../../.gitbook/assets/image (6).png" alt=""><figcaption><p>Image showing example API key from printer settings</p></figcaption></figure>

***

### **Step 2: Install PushPrinter on Android**

1. **Download PushPrinter** from the _Google Play Store_.
2. Open the app after installation.
3. Press the **settings icon ⚙️**, then select **Default**.

***

### **Step 3: Add and Configure a Printer on Android**

1. Tap **"+" (Add Printer)** to configure a printing service.
2. Select **Bluetooth** or **Network (for IP Printer)**:
   * If using **Bluetooth**, the app will **automatically scan** for available printers.
     * Ensure your printer is powered on and in pairing mode.
     * Select your printer from the list.
   * If using a **Network (IP Printer)**, select **"Network"** and **manually enter the printer's IP address**.
     * Ensure the printer and Android device are on the same Wi-Fi network.
3. Enter the **API Key** from your CloudWaitress dashboard. The API key can be found on the restaurant's printer settings. (Settings > Receipt Printing)
4. If prompted, enter the default printer PIN (**0000** or **1234**).
5. Confirm that the **printer status is "Connected"** in your CloudWaitress dashboard.
6. Once all the details are filled out, check the status of the printer on your restaurant’s settings. Make sure it appears as connected.

<div align="left" data-full-width="true"><figure><img src="../../.gitbook/assets/push3.png" alt="" width="318"><figcaption><p>Press the "+” sign on the top to configure a printing service. Make sure that the printer is on.</p></figcaption></figure></div>

<div align="left"><figure><img src="../../.gitbook/assets/image (10).png" alt="" width="210"><figcaption><p>Pair the Android device to the printer via Bluetooth</p></figcaption></figure></div>

<div align="left"><figure><img src="../../.gitbook/assets/image (11).png" alt="Android-test-print-on-pushprinter" width="204"><figcaption><p>Once it’s successfully connected, a test print will be sent to the printer.</p></figcaption></figure></div>

<div align="left"><figure><img src="../../.gitbook/assets/image (13).png" alt="" width="208"><figcaption><p>Fill out Printer Details such as the Printer Name, API Key and Number of Copies.</p></figcaption></figure></div>

<div align="left"><figure><img src="../../.gitbook/assets/image (7) (1).png" alt="" width="375"><figcaption><p>Printer status showing connected</p></figcaption></figure></div>

***

### **Step 4: Test Printing**

1. Visit the **Orders Page** in CloudWaitress.
2. Select an order, then choose **"Print"**.\
   (We recommend printing both short and long orders to ensure that there is nothing being cut out vertically.)
3. If you enabled **auto-printing**, place a test order to ensure automatic printing is enabled.

![](<../../.gitbook/assets/image (5).png>)

***

## Troubleshooting: Common Issues & Fixes

{% hint style="success" %}
**Contact Us**

We have successfully setup 100's of printers; there is a good chance we can save you lots of headaches, so please don't hesitate to [contact us via chat](https://www.cloudwaitress.com).
{% endhint %}

#### **1. Sides of the receipt are cut off**

✅ Adjust the **Paper Scale Factor** to **1.7** and test again.

#### **2. Invalid API Key**

✅ Verify that the **API key matches** the one in your CloudWaitress printer settings.

#### **3. Printer is connected, but no printouts**

✅ Restart the Android device and **ensure Android detects the printer** in Bluetooth or Wi-Fi settings.

#### **4. Unable to authenticate printing**

✅ Check your **internet connection** and try again later. Try restarting your device. Try printing to your printer from other computer programs such as your browser.



{% hint style="info" %}
Get started for free at [www.cloudwaitress.com/signup](https://www.cloudwaitress.com/signup/)
{% endhint %}



