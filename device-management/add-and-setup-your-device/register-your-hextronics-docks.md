---
description: >-
  Keywords - Add Device, Registration, Hextronics Atlas, DJI Matrice 300 RTK,
  DJI Matrice 350 RTK, Hextronics Universal, DJI Mavic 3 Enterprise Series
---

# Register Your Hextronics Docks

## Overview

Follow the steps in this guide to add your Hextronics Atlas dock with its Matrice 300 RTK/350 RTK drone, or Hextronics Universal with its Mavic 3 Enterprise Series drone (collectively referred to as a Device) to FlytBase.&#x20;

### Site Evaluation

How to choose a site for setting up your Hextronics Docking Station?

* Ensure there is a clear and unobstructed path between the Docking Station and the Safe Location (Alternate Landing Location).

<figure><img src="../../.gitbook/assets/image (1).png" alt=""><figcaption><p>There must be an unobstructed path between the Dock's location and the safe location</p></figcaption></figure>

* The Location of the Dock must have healthy RTK convergence for the drone.&#x20;

{% hint style="info" %}
To check whether the RTK signal strength is healthy at the Dock's location, connect the RTK base station/NTRIP using DJI Pilot app.

Refer to this [video](https://youtu.be/-pzmpmiD9fs?si=5G510rpJGs5L8YkE) to understand this process.
{% endhint %}

## Prerequisites

Before you begin, ensure that you have set up the Hextronics dock, drone, and Remote Controller (RC) as per the instructions in the Hextronics Quick Start Guide.

Furthermore, ensure you have completed the following steps for setting up your FlytBase Dashboard before beginning the Hextronics Docking Station registration process.

1. [Create or join an organization](../../getting-started-with-your-flytbase-account/creating-an-organization.md)
2. [Set up a site](../../getting-started-with-your-flytbase-account/site-management.md)
3. Keep your activation code handy

## Setting up your DJI Remote Controller (RC Plus or RC Pro)

As the first step of the Device registration process, we set up the RC for working with FlytBase. At the end of this section, you will have set up your RC Plus or RC Pro for operations with FlytBase.&#x20;

### Step 1: Install FlytBase Application (APK file)

{% embed url="https://youtu.be/UzBbnRbhRYM" %}
\[Video] Downloading and Installing FlytBase App using APK
{% endembed %}

* **Prepare the RC:** Switch on the RC and set it up according to DJI instructions.
  * Make sure that your DJI Drone is registered with DJI.
  * RC must be set up as 'Controller A'.
* **Download and Install FlytBase App: D**ownload the relevant file for FlytBase App (.apk extension) as per your Dock and Drone:
  * Hextronics Atlas and DJI M350 RTK: [https://flyt.link/Atlas-M350](https://flyt.link/Atlas-M350)
  * Hextronics Atlas and DJI M300 RTK: [https://flyt.link/Atlas-M300](https://flyt.link/Atlas-M300)
  * Hextronics Universal and DJI Mavic 3 Enterprise: [https://flyt.link/Uni-Mavic](https://flyt.link/Uni-Mavic)

{% hint style="info" %}
Use the Browser on your DJI RC Plus/RC Pro to download the relevant APK using the above links.
{% endhint %}

* **Install the APK:** Locate the downloaded file on the RC and click on it to install the FlytBase app. Once installed, open the FlytBase app to verify installation.

### Step 2:  Bind Drone to RC (Optional)

This step is to be completed if the Drone and the RC have not been bound already.

* Power on the Drone and RC.
* Hold the power button to switch the drone to Bind mode.
* On the RC, open the FlytBase app, and click the Bind button. Follow the on-screen instructions to initiate the Drone and RC binding process.
* Once completed, the FlytBase app will display the Drone as Connected.

{% hint style="info" %}
- For instructions on binding the M350 RTK to its remote controller, please see page 56 of the [Matrice 350 RTK User Manual](https://dl.djicdn.com/downloads/matrice_350_rtk/20240814/Matrice_350_RTK_User_Manual_v1.2_en.pdf).
- For binding the M350 RTK to its remote controller, refer to page 46 of the [M300 RTK User Manual](https://dl.djicdn.com/downloads/matrice-300/20230518UM/M300_RTK_User_Manual_EN_v4.0.pdf).
- For binding the Mavic 3 Enterprise to its remote controller, consult pages 59 and 60 of the [DJI Mavic 3E/3T User Manual](https://dl.djicdn.com/downloads/DJI_Mavic_3_Enterprise/20240814/DJI_Mavic_3E_3T_User_Manual_EN.pdf).
{% endhint %}

### Step 3: Set FlytBase App to Auto Start

FlytBase App installed in the RC must be set to auto-start whenever the RC is powered on for automated dock-drone operations using FlytBase. To enable this, follow the instructions below:



{% embed url="https://youtu.be/1Flr4Ji3kCQ" %}

* Navigate to Android Settings on the RC.
* In the Settings menu, select Apps and Notifications.
* Select the Auto-Start Application option and choose FlytBase from the list of available apps. This will ensure FlytBase launches automatically whenever the RC is powered on.
* Restart the RC to verify the Auto-Start of the FlytBase app.

### Step 4: Install AirDroid (Enables Remote Access)



{% embed url="https://youtu.be/ZwHuau95E7s" %}
\[Video] Installing AirDroid and enabling permissions
{% endembed %}

* **Download and Install AirDroid Business App:** Download the AirDroid Business app from the following link:[ ](https://airdroid.at/679441)[https://flyt.link/Airdroid](https://flyt.link/Airdroid).&#x20;
  * Open the location of the downloaded file (.apk file extension), and click on it to install.
  * Once installed, open the AirDroid app.
* **Setup AirDroid App:** Enter a new device name when prompted.&#x20;
  * Grant all the necessary permissions as mentioned below:&#x20;
    * Remote control
      * View mode
      * Remote camera
      * File transfer
      * Device location
      * Lock and factory reset
      * App list and uninstall
      * Ignore battery optimization

These permissions can also be managed in Android **Settings** -> **Apps and Notifications** -> **Biz Daemon** -> **Permissions and Advanced settings** on the RC.

## Device Registration

### Before You Start

Before starting the registration process, please ensure that:

* The Dock and Drone are physically accessible.
* The Dock and RC should be connected to the Internet.

{% hint style="warning" %}
During Device registration, only one unregistered Dock should be on the same network as the RC.
{% endhint %}

### Adding a Device

{% embed url="https://youtu.be/_qdoQaKxUfw" %}
\[Video]  Step 1 - Adding a Device on Dashboard and generating MQTT credentials
{% endembed %}

{% embed url="https://youtu.be/Q5HKmlFhr8k" %}
\[Video] Step 2- Registering the Device using MQTT credentials on RC
{% endembed %}

* **Access the Device Management window:** On the FlytBase Dashboard, click on ![](<../../.gitbook/assets/Hamburger Menu.svg>) to open the **Navigation Drawer**, and select **Devices**. This will open the **Device Management** window.
* **Add a New Device:** Click on <img src="https://lh5.googleusercontent.com/1NmivB7btnzbgjplC3RRTtRQ6OTrcjiX7krecQbSg0uZEGl9ghSOEnhWHAxUyBbAURkoWMud24yUmGpwjHF261NAmk8ce8HLo3UQF3l5m7aTWV7O0XccS4tVPApWHCDVipHU6v8-nrPaMW8x9RLMzw" alt="" data-size="line"> to add a new Device. The **Add Device** dialog box will appear.
* **Step 1 - Enter Device Details:** Enter suitable names for the new Dock and Drone. Also, select the **Site** with which the Dock and Drone would be associated. Once done, click on **Next**.
* **Step 2 - Prepare Device:** Open the **FlytBase app** on the RC. Power on the Dock and confirm that both the RC and the Dock are connected to the Internet. Once confirmed, click on **Next** on the Dashboard to proceed to **Step 3**.
* **Step 3 - Enter MQTT Credentials:**
  * **Step 3** of the Registration process will display the **MQTT credentials**.
  * In the **FlytBase app** on the RC, click on <img src="../../.gitbook/assets/image (183).png" alt="" data-size="line">. On the page that opens, **enter the MQTT credentials** as displayed on the Dashboard and click on **Register**.
* **Complete Registration:** Once the registration process is complete, the RC will switch to Cockpit view. Click the Back button on the RC to return to the Home screen. The RC should indicate that it is connected to both the network and Dock OS.
* **Finalize Registration:** On the Dashboard, click **OK** to finish the registration process.&#x20;

Once registration is complete, the Device will be visible in the Device Management window.

{% hint style="warning" %}
Before using the Device for operations, you need to [activate the FlytBase subscription](../activating-device-subscription.md).&#x20;
{% endhint %}
