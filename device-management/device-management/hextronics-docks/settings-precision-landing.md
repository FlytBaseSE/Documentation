---
description: >-
  Keywords - Vision Precision Landing, RTK Precision Landing, Trigger Height,
  Landing Threshold, Guided Final Approach, Precision Landing settings
---

# Settings - Precision Landing

## Overview

The FlytBase Precision Landing module enables drones to land accurately on landing tags located on docking stations or landing pads with centimeter-level precision. This is essential to avoid collisions and damage when landing in the docking station.

For precision landing, the drone must be above the landing tag to activate visual or RTK-based guidance, ensuring a safe and precise landing with minimal manual intervention.&#x20;

## Precision Landing Parameters

To configure Visual or RTK-based Precision Landing, the following parameters need to be set:

* **Trigger Height:** This is the height above the docking station where the drone initiates the Precision Landing procedure. It can be set to 5, 10, or 15 meters, depending on the size of the landing tag and the camera resolution.
* **Landing Threshold:** This is the altitude at which the drone positions itself over the landing area before executing the DJI Land command. The drone does not perform any recovery maneuvers after reaching this threshold.
* **Guided Final Approach:** This setting determines whether the drone will be guided all the way to the ground or just to the Landing Threshold height before executing the DJI Land command. Enabling this setting ensures continuous guidance to the ground for a more precise landing, while disabling it stops guidance at the Landing Threshold height.

## Precision Landing Settings

To configure Precision Landing parameters, follow these steps:

* Navigate to **Devices** -> _Select your device_ -> **Settings**, and select **Precision Landing**.
* Choose **Vision** or **RTK Precision Landing** mode.
* Set the **Trigger Height** to 5, 10, or 15 meters for the selected mode.
* Set the **Landing Threshold** altitude for the selected mode.
* Toggle the option for **Guided Final Approach** on or off for the selected mode.

<figure><img src="../../../.gitbook/assets/precision landing settings.jpg" alt=""><figcaption><p>Precision Landing settings </p></figcaption></figure>

{% hint style="warning" %}
Precision Landing settings can be done only when the drone is powered on.
{% endhint %}

{% hint style="info" %}
After completing Precision Landing settings, refer to the guide on calibrating the Precision Landing module for repeatable and reliable autonomous landings.
{% endhint %}

