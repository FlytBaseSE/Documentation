---
description: >-
  Keywords - RTDS Altitude, RTSL Altitude, GTSA Altitude, Dock Location, Safe
  Location, Automate Operations
---

# Settings - Drone and Dock

## Overview

Drone and Dock Settings allow you to configure various parameters necessary for safe operations. As part of Drone settings, you can set the altitudes at which the Drone would return to the Dock or its Safe Location. You can also set the Safe location and Dock location from Dock settings.&#x20;

## Drone Settings

<figure><img src="../../../.gitbook/assets/image (591).png" alt=""><figcaption><p>Drone Control Settings</p></figcaption></figure>

### 1. Return to Docking Station (RTDS)

**Significance:** At the end of all missions, it is recommended that the final action is set to Return to Docking Station (RTDS). This ensures the safe termination of all flight operations.

* **RTDS Altitude:** Set the altitude at which the drone would perform RTDS. The drone would ascend/descend to this altitude from its present altitude before moving towards the Docking Station.
* **RTDS Speed:** Set the speed at which the drone would perform RTDS. Once the drone has achieved its RTDS altitude, it will move towards the Docking Station at the speed set here.

{% hint style="warning" %}
RTDS Altitude should be less than the Maximum Altitude set in Devices -> Zones for that particular Device.&#x20;
{% endhint %}

### 2. Return to Safe Location (RTSL)

**Significance:** In an event where the Docking Station is not suitable for landing, the drone would land at the Safe Location. This ensures proper retrieval of drone even if it has not landed in the Docking Station.&#x20;

* **RTSL Altitude:** Set the altitude at which the drone would perform RTSL. The drone would ascend/descend to this altitude from its present altitude before moving towards the Safe Location.

{% hint style="warning" %}
RTSL Altitude should be less than the Maximum Altitude set in Devices -> Zones for that particular Device.&#x20;
{% endhint %}

### 3. Go to Safe Altitude

**Significance:** In case of a situation where an airspace threat is detected, the drone may be instructed to stop all operations and descend to a safe altitude, and then hover at its current position. This provides users with a means to respond to immediate threats and maintain the safety of all assets.

* **Safe Altitude:** Set the minimum altitude at which the drone can hover without colliding with any object/structure in the area of operation. The drone will descend to this altitude and hover at its current location whenever GTSA is triggered.&#x20;
* **Speed:** Set the speed with which the drone would descend to the safe altitude.

{% hint style="warning" %}
Safe Altitude should be lower than the Maximum Altitude set in Devices -> Zones for that particular Device. It should also be higher than the highest structure/object in the area of operation.
{% endhint %}

{% hint style="warning" %}
All altitudes are measured relative to the take-off location, i.e., the Docking Station. This is also referred to as the RLT reference for measuring altitude.
{% endhint %}

## Dock Settings

<figure><img src="../../../.gitbook/assets/image (592).png" alt=""><figcaption><p>Dock Settings</p></figcaption></figure>

### Location

**Significance:** It is necessary for operations that the drone knows where the Docking Station is, and where it can land if landing on Docking Station is not possible. These locations can be set on the FlytBase Dashboard as part of Dock Settings

* **Dock Location:** You can set the Dock's location on the map. The area needs to be set every time the Dock is moved from its current position.
* **Safe Location:** You can also set the Safe Location for a particular Dock. The drone would land here in case the Dock is not available for landing.&#x20;

### Automate Operations

**Significance:** Docks that have pre- and post-takeoff/landing routines require manual input to complete these routines. Automate Operations command makes these routines autonomous.

* **Automate Operations toggle:** enable or disable Automated Operations for any Dock.

### Landing Safety

{% hint style="warning" %}
Only certain Docks support this feature.
{% endhint %}

**Significance:** Sometimes the drone might land on the Dock incorrectly. Initiating a post-landing routine in such cases may damage the drone and the Dock. Thus, some Docks provide a feature to verify the proper landing of the drone before initiating post-landing routine.

* **Landing verification toggle:** enable or disable landing verification. When enabled, the Dock will stay open in case an incorrect landing is detected.

