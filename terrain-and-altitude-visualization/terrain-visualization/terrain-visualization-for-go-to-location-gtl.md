---
description: >-
  A comprehensive guide to using the Terrain Visualization feature, which
  provides an estimate of the terrain features along your flight path, helping
  you safely navigate to your Go To Location (GTL).
---

# Terrain Visualization for Go To Location (GTL)

## Setting up your reference altitude during GTL (Go To Location) missions

### **Choose Your Altitude Reference** between:

* **Relative to Takeoff (RTL):** Measures altitude relative to the drone’s launch point.
* **Above Ground Level (AGL):** Adjusts altitude dynamically based on terrain variations.

<figure><img src="../../.gitbook/assets/Fleet view-2.png" alt=""><figcaption><p>Setting the reference altitude for the destination </p></figcaption></figure>

* Access the detailed terrain profile graph to analyze elevation changes and compare the **Go To Location (GTL)** target elevation for precise and safe navigation.

<figure><img src="../../.gitbook/assets/Fleet view-3.png" alt=""><figcaption><p>Visualization of the terrain elevation before launching GTL mission</p></figcaption></figure>

### Pre Flight Caution Alerts and Warnings

**Caution Alerts and Warnings:** If the planned flight altitude exceeds limits or creates a conflict with the terrain, FlytBase provides an immediate warning, ensuring compliance with safety protocols.

{% hint style="warning" %}
Operators would be able to see an advance warning under the Terrain Profile Graph in case the flight path would come in close contact with the ground (within 20 meters) at any point when the Go To Location (GTL) point is selected. In this case a review of the flight path is strongly recommended.
{% endhint %}

<figure><img src="../../.gitbook/assets/Fleet view-8.png" alt=""><figcaption><p>Caution due to ground and flight route distance</p></figcaption></figure>

{% hint style="warning" %}
Operators would be able to see an advance warning over the Terrain Profile Graph in case any point on flight path exceeds the maximum altitude limit specified for the drone in device settings when Go To Location (GTL) point is selected. In this case a review of the flight path is strongly recommended.
{% endhint %}

<figure><img src="../../.gitbook/assets/Fleet view-9.png" alt=""><figcaption><p>Caution due to flight altitude exceeding maximum limit</p></figcaption></figure>

{% hint style="danger" %}
Operators would see a warning under the Terrain Profile Graph in case any point on the flight path is within collision proximity with the ground when the Go To Location (GTL) point is selected to mitigate the collision risk. In this case, you would need to redefine the altitude parameter.
{% endhint %}

<figure><img src="../../.gitbook/assets/Fleet view-10.png" alt=""><figcaption><p>Warning due to possibility of ground collision</p></figcaption></figure>
