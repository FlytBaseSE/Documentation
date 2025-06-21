---
description: >-
  This feature allows you to track the altitude information in-flights ensuring
  better visibility and safety while your drone is performing automated missions
  or during manual manual flights.
---

# In-Flight Altitude Visualization

### Overview

The **In-Flight** **Altitude Visualization** feature provides real-time altitude information relative to the drone’s current flight level. It helps operators track key altitude parameters such as remaining ascent capability, proximity to the docking station, and distance from the ground during missions and manual flights.

### In-Flight Altitude Visualization

{% hint style="info" %}
All altitude-related parameters on the **Drone Card** are referenced to the drone’s **current altitude**:

* **Positive values** indicate altitudes **above** the drone’s current altitude.
* **Negative values** indicate altitudes **below** the drone’s current altitude.
{% endhint %}

* The following parameters are displayed as part of the altitude visualization in the drone card:&#x20;
  * **Max Alt:** Displays the remaining distance the drone can ascend before reaching its maximum altitude.
  * **RTDS** (Return to Dock Station): Shows the altitude difference between the drone’s current altitude and the altitude at which it will initiate the approach to the docking station.
  * **Dock**: Indicates the drone’s altitude relative to the docking station’s altitude.
  * **Ground**: Reflects how high the drone is above the ground level.

<figure><img src="../.gitbook/assets/Image 26-02-25 at 2.34 PM (1).jpeg" alt=""><figcaption><p>Altitude Visualization informing in the Drone Card</p></figcaption></figure>

{% hint style="success" %}
The Max Alt and RTDS altitude values can be set in the drone's device settings.
{% endhint %}

### Accessing In-Flight Altitude Visualization &#x20;

* Navigate to the '**Fleet**' tab in the Navigation Drawer on the Operations Dashboard.

<figure><img src="../.gitbook/assets/Image 26-02-25 at 4.26 PM.jpeg" alt=""><figcaption></figcaption></figure>

* Click on the card of the drone which you wish to control.
* In the drone's detailed view, locate the 'Missions' control panel.
* Select the desired **path/grid mission** from the list or provide a **Go To Location (GTL)** command.
* Once the drone takes off, you would be able to see the real-time altitude visualization in the fleet view.

<figure><img src="../.gitbook/assets/Image 26-02-25 at 1.30 PM.jpeg" alt=""><figcaption><p>Altitude Visualization in Fleet View</p></figcaption></figure>

* You can view this information in the cockpit view as well.&#x20;

<figure><img src="../.gitbook/assets/Image 26-02-25 at 2.35 PM.jpeg" alt=""><figcaption><p>Altitude Visualization in Cockpit View </p></figcaption></figure>

### Warnings

{% hint style="warning" %}
When the drone is within 20 meters to the ground level such as events like landing, you would see a warning appear.
{% endhint %}

<div align="center" data-full-width="false"><figure><img src="../.gitbook/assets/Image 26-02-25 at 2.43 PM.jpeg" alt="" width="341"><figcaption><p>Ground Level Warning</p></figcaption></figure></div>

{% hint style="warning" %}
When the drone is within 20 meters to approaching the maximum altitude, you would see a warning with the highlighed distance of possible ascent available.&#x20;
{% endhint %}

<div align="center"><figure><img src="../.gitbook/assets/Untitled design-12.png" alt=""><figcaption><p>Maximum Altitude Warning</p></figcaption></figure></div>

