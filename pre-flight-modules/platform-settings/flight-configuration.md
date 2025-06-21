---
description: >-
  Set the default flight characteristics of the drones added to the
  Organization.
---

# Flight Configuration

In the **Flight Configuration** tab, you can define the default flight characteristics for drones within your Organization, ensuring they operate safely and predictably during standard missions unless specified otherwise.

### Default Settings&#x20;

These settings define the standard flight speed and altitude for the drone's missions and are recommended whenever a new mission is created.

* **Flight Speed:** This is the ideal speed at which drones should perform their missions. It is applied to all drones in the Organization.&#x20;

{% hint style="info" %}
Flight Speed settings do not apply to Go-to Location missions (for DJI Dock).
{% endhint %}

* **Flight Altitude:** This is the altitude at which it is safe to conduct all missions, including Go-to Location. It is applied to all drones in the Organization.

### Advance Settings

To control the drone's responsiveness under manual control, you can adjust the rate at which the drone moves in any direction. These adjustments are available in two modes: Default and Adaptive.

* **Default Mode**: In this mode, the preset speeds are consistently applied to the drone under manual control, regardless of the altitude.

<figure><img src="../../.gitbook/assets/capture_20240419191604283.bmp" alt=""><figcaption><p>Flight Configuration: Default Settings (Green) and Advance Settings - Default Mode (Red)</p></figcaption></figure>

* **Adaptive Mode**: In this mode, you can specify a cutoff altitude. Above this altitude, the drone can be faster and more responsive. Below this altitude, the drone will be slower, allowing for more precise control.

{% hint style="warning" %}
Advance Settings are specific to each Member of the Organization.
{% endhint %}

**Configurable Parameters in Advance Settings**:

* **Throttle**: This controls the speed at which the drone moves vertically up or down, measured in meters per second.
* **Drone Pitch and Roll**: This setting adjusts the speed at which the drone moves forward, backward, or side to side, measured in meters per second.
* **Drone Yaw**: This parameter controls the rate at which the drone rotates around its vertical axis, measured in degrees per second.
* **Altitude Threshold**: The altitude at which the drone would change its speeds (for **Adaptive Mode** only).

<figure><img src="../../.gitbook/assets/capture_20240419191956647.bmp" alt=""><figcaption></figcaption></figure>
