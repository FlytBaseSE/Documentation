---
description: >-
  Emergency Landing feature allows operators to perform safe, controlled
  landings in case of emergencies, enhancing operational safety.
---

# Emergency Landing

## Overview

FlytBase now supports **Emergency Landing** designed to ensure safe drone recovery in case of emergency situations, such as **dock malfunction** or poor weather. This capability enhances operational safety by allowing operators to perform controlled landings. This feature is critical for automated operations—especially BVLOS, security, and industrial inspections—where minimizing risk and downtime is essential.

## Key Features

* **Dashboard-Based Emergency Landing Access**\
  Operators can initiate emergency landings directly from the FlytBase Operations Dashboard. Simply select the drone, navigate to the **Missions** panel, and access the **Land** button once the drone is armed.
* **One-Click Emergency Descent**\
  The **Land** button allows the drone to descend and safely land at its current in-flight location. A confirmation prompt ensures that landing is deliberate and controlled.
* **Location Tracking for Recovery**\
  Post-landing, the system displays the **last known location of the drone**, including real-time map positioning and GPS coordinates, to assist field teams with quick recovery.

## Steps to perform Emergency Landing

### **Step 1: Access the Drone Controls**

* Navigate to the **Operations Dashboard**.
* Click on the card representing the drone you wish to control to open its detailed view.

### **Step 2: Navigate to Mission Controls**

* Within the drone's detailed view, locate the **Missions** control panel.
* Choose the appropriate mission (Path/Grid) from the list, or issue a **Go To Location (GTL)** command as needed.
* Once the drone is **armed**, additional control options will become visible in the drone control panel.

<figure><img src="../../.gitbook/assets/Fleet view (1).png" alt=""><figcaption><p>Fleet View during Go To Location (GTL) Command</p></figcaption></figure>

### **Step 3: Initiate Emergency Landing**

* Click the **Land** button on the drone control panel.
* A confirmation prompt will appear asking you to confirm the emergency landing.

<figure><img src="../../.gitbook/assets/Fleet view-1.png" alt=""><figcaption><p>Confirm Emergency Landing</p></figcaption></figure>

* Confirming this will immediately initiate landing at the drone’s **current location**.

{% hint style="danger" %}
**Important:** Before confirming, ensure the area directly below the drone is clear of obstacles, people, and hazards to prevent damage or injury.
{% endhint %}

### **Step 4: Monitor Landing**

* The drone will descend and safely land at the current location.
* The **last known location** of the drone, along with its **latitude and longitude**, will be displayed on the map for tracking and retrieval.

<figure><img src="../../.gitbook/assets/Fleet view-3 (1).png" alt=""><figcaption><p>Last Known Location Of Drone After Emergency Landing</p></figcaption></figure>

### **Step 5: Acknowledge Recovery**

* Once the drone has been safely retrieved, click the **Acknowledge** button.

<figure><img src="../../.gitbook/assets/Fleet view-5 (1).png" alt=""><figcaption><p>Confirming Drone Recovery</p></figcaption></figure>

* Upon confirming recovery, the drone panel and dashboard will reset to their normal state, ready for the next operation.

<figure><img src="../../.gitbook/assets/Fleet view-6.png" alt=""><figcaption><p>Reset State After Confirming Recovery</p></figcaption></figure>
