---
description: >-
  This section will guide you on the step-by-step process on setting up a
  bluetooth printer.
---

# Setup Printing Using Bluetooth Printer

{% embed url="https://drive.google.com/file/d/1Px4Sn_7b-ftCAfR7CFe87y6WE5F8SAEQ/view?usp=sharing" %}

### Step 1: Create a Printer Configuration

1. Open your [**CloudWaitress dashboard**](https://admin.cloudwaitress.com).
2. Go to **Settings > Receipt Printing > Create Printer**.
3. Fill in:
   * **Printer Name -** i.e. "Android Kitchen Printer"
   * **Printing Method:** Set to _ESCPOS_
   * **Printing Type:** Use _ESCPOS Image_ for best results. (Note that some older printers may not support this method and ESCPOS Text Only can be used in these cases).
   * **Paper Scale Factor:** Adjust to **1.7** if text is cut off.
4. Click **"Save"** and copy your unique **API key** (needed later).

<figure><img src="../../.gitbook/assets/Screenshot 2025-11-30 at 4.24.51 AM.png" alt="" width="375"><figcaption></figcaption></figure>

<figure><img src="../../.gitbook/assets/Screenshot 2025-11-30 at 4.25.20 AM.png" alt="" width="276"><figcaption></figcaption></figure>

### **Step 2: Install PushPrinter on Android**

1. **Download PushPrinter** from the _Google Play Store_.
2. Open the app after installation.
3. Press the **settings icon ⚙️**, then select **Default**.

### **Step 3: Add and Configure a Printer on Android**

1. Tap **"+" (Add Printer)** to configure a printing service.
2. Select **Bluetooth** or **Network (for IP Printer)**:
   * If using **Bluetooth**, the app will **automatically scan** for available printers.
     * Ensure your printer is powered on and in pairing mode.
     * Select your printer from the list.
3. Enter the **API Key** from your CloudWaitress dashboard. The API key can be found on the restaurant's printer settings. (Settings > Receipt Printing)

<figure><img src="../../.gitbook/assets/Screenshot 2025-11-30 at 4.25.31 AM.png" alt="" width="375"><figcaption></figcaption></figure>

4. If prompted, enter the default printer PIN (**0000** or **1234**).
5. Confirm that the **printer status is "Connected"** in your CloudWaitress dashboard.
6. Once all the details are filled out, check the status of the printer on your restaurant’s settings. Make sure it appears as connected.
7. Click "Test Print" if setting up is successful, it will do a test print
8. Once successful, do an order test

* Go to the ordering site and do a test order
* Enable auto-printing to ensure automatic printing





{% hint style="danger" %}
Please email [support@cloudwaitress.com](mailto:support@cloudwaitress.com) or use the chat support feature to get assistance managing this feature.
{% endhint %}
