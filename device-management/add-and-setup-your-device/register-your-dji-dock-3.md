---
description: >-
  Keywords: Add Device, Registration, DJI Dock 3,  RC Plus 2, Third Party Cloud
  Service, MQTT
---

# Register Your DJI Dock 3

## Overview

This guide explains how to register your DJI Dock 3 along with its associated drone on FlytBase. The process is designed to be straightforward, ensuring that both the dock and the drone are correctly configured to connect with our platform. Follow these steps carefully to ensure a successful registration.

## Device Registration

### Before You Start

Before beginning the registration process, please make sure that:

* **Physical Access:** Both the DJI Dock 3 and its paired drone are easily accessible.
* **Bound Devices:** The drone and dock are already bound together.
* **Power & Connectivity:**
  * The dock is connected to a stable internet connection.
  * The drone is powered on throughout the registration process.
* **RC Plus 2 Ready:** You have the RC Plus 2 available and it’s ready to connect to the docking station.
* **Preparation:** Familiarize yourself with the "DJI Enterprise" app on the RC Plus 2, as this will be used to complete the configuration.

### Adding a Device

Follow these steps to register your DJI Dock 3 on FlytBase:

1. **Access Device Management:**
   * Log in to your FlytBase Dashboard.
   * Open the Navigation Drawer and select **Devices** to access the Device Management window.
2. **Initiate Device Registration:**
   * Click on **Add New Device** to open the registration dialog.
   * In Step 1, enter appropriate names for your new dock and drone. Also, choose the Site with which they will be associated, then click **Next**.
3. **Connect the RC Plus 2:**
   * Connect the RC Plus 2 to your DJI Dock 3.
   * Launch the **DJI Enterprise** app on the RC Plus 2.
   * On the app’s main screen, select your dock’s image or name to open the **Cloud Service Configuration** window.
4. **Configure Cloud Service:**
   * In the Cloud Service Configuration window, select **Third Party Cloud Service** from the drop-down menu.
   * Enter the following details:
     * **MQTT URL:** ssl://cloud.flytbase.com:8883
     * **MQTT Credentials:** These are dynamically generated. To obtain the credentials specific to your device, go to **FlytBase Operations Dashboard > Devices > Add**, then set up the name and site for your drone. The generated MQTT credentials will be displayed for you to enter.
     * **Organisation Code**: W
     * **Binding Code**: qwe
   * Confirm the settings by clicking **OK**. The RC Plus 2 should display a confirmation indicating that the device has been successfully registered.
5. **Complete the Registration:**
   * Return to the FlytBase registration dialog and click **Next** or **Finish** (as applicable) to complete the process.
   * Once completed, the DJI Dock 3 and its associated drone will appear in the Device Management window.
   * After this activate the subscription for your device in the Management Console by heading to Device Subscription.
6. **Post-Registration Step:**
   * It is recommended to reboot your DJI Dock 3 after registration. Disconnect the RC Plus 2 and then perform a physical reboot of the dock.

### Final Notes

* **Subscription Activation:** Before using your DJI Dock 3 for operations, ensure that you activate your FlytBase subscription.
* **Support:** If you encounter any issues or have questions during the setup process, please contact our support team.&#x20;
