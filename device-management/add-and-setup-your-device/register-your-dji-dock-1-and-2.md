---
description: >-
  Keywords - Add Device, Registration, DJI Dock, Matrice 30/30T, DJI Dock 2,
  Matrice 3D/3TD, MQTT.
---

# Register Your DJI Dock 1 and 2

## Overview

To add your DJI Dock with its Matrice 30/30T drone, or DJI Dock 2 with its Matrice 3D/3TD drone (collectively referred to as a Device) to FlytBase, follow the steps outlined in this guide.&#x20;

## Device Registration

### Before You Start

Before starting the registration process, please ensure that:

* The Dock and Drone are physically accessible.
* The Dock and Drone are powered on and bound together.
* A USB A-to-C cable is available to connect the Dock to the RC.

### Adding a Device

* **Access the Device Management window:** On the FlytBase Dashboard, click on ![](<../../.gitbook/assets/Hamburger Menu.svg>) to open the **Navigation Drawer**, and select **Devices**. This will open the **Device Management** window.
* **Add a New Device:** Click on <img src="https://lh5.googleusercontent.com/1NmivB7btnzbgjplC3RRTtRQ6OTrcjiX7krecQbSg0uZEGl9ghSOEnhWHAxUyBbAURkoWMud24yUmGpwjHF261NAmk8ce8HLo3UQF3l5m7aTWV7O0XccS4tVPApWHCDVipHU6v8-nrPaMW8x9RLMzw" alt="" data-size="line"> to add a new Device.
* **Step 1:** The **Add Device** dialog box will appear. In **Step 1**, enter suitable names for the new Dock and Drone. Also, select the **Site** with which the Dock and Drone would be associated. Once done,  click on **Next**.
* **Step 2:** As part of **Step 2,** connect the RC to the Dock. This will open the **On-site Debugging** window of the **DJI Pilot** app on the RC.
  * On the RC, click on the name below the image of the Dock on the left side of the screen. This will take you to the **Cloud Service Configuration** window. Set the **Cloud service** to **Third-Party Cloud Service** from the drop-down list.
* **Step 3:** Proceed to **Step 3** in the dialog box by clicking **Next**. In this step, the **MQTT Credentials** required for Device Registration will be displayed.
  * Enter these credentials exactly on the RC in the **Cloud Service Configuration** window. Once done, click **OK**. The RC will indicate that the Device has been successfully registered.
* **Complete the Registration Process:** Click OK on the dialog box to close it and complete the Device registration process.

Once registration is complete, the Device will be visible in the Device Management window.

{% embed url="https://youtu.be/rCefaki8I30" %}
DJI Dock Setup on FlytBase
{% endembed %}

{% hint style="info" %}
It is recommended to reboot your DJI Dock once it has been registered on FlytBase. (disconnect RC, then physically reboot)
{% endhint %}

{% hint style="warning" %}
Before using the Device for operations, you need to [activate the FlytBase subscription](../activating-device-subscription.md).
{% endhint %}
