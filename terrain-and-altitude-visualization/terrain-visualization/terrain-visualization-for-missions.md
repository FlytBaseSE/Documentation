---
description: >-
  A comprehensive guide to using the Terrain Visualisation feature, which
  provides an estimate of the terrain features along your flight path, helping
  you navigate safely throughout your mission.
---

# Terrain Visualization for Missions

## Selecting your mission

* Navigate to the **Fleet** tab in the Navigation Drawer.
* Click on the card of the drone which you wish to control.
* In the drone's detailed view, click on the **Missions** button in the control panel.
* Select the desired path/grid mission from the list and click on next.

<figure><img src="../../.gitbook/assets/Fleet view-4.png" alt=""><figcaption><p>Selecting the Mission</p></figcaption></figure>

## Terrain Visualisation Before Mission Execution

{% hint style="warning" %}
Terrain Visualisation does not work for Scheduled missions. Users should verify by planning to execute the mission once before scheduling it.
{% endhint %}

### 1. Path Missions

Before executing Path missions, you can preview the altitude of each waypoint using the **terrain profile graph. This will allow you to a**ssess altitude variations over the flight path using the RLT altitude reference on the Y-axis, and the terrain outline along the flight path.&#x20;

This allows for precise comparison of elevation changes at **individual waypoints**, ensuring safe flight path for mission.

<figure><img src="../../.gitbook/assets/Screenshot 2025-02-10 at 7.20.17 PM (1).png" alt=""><figcaption><p>Terrain Elevation preview for selected waypoint mission</p></figcaption></figure>

### 2. Grid Missions

A clear altitude preview for all grid points will be visible using the **terrain profile graph**, enabling you to compare elevation changes along the flight path.&#x20;

<figure><img src="../../.gitbook/assets/Screenshot 2025-02-10 at 7.21.36 PM.png" alt=""><figcaption><p>Terrain Elevation preview for selected grid mission</p></figcaption></figure>

### 3. Breakpoint Missions (Resuming incomplete missions)

For a waypoint or grid mission with a breakpoint, you would be able to view the resuming point on the flight path labelled as **B. It will also be indicated on** the Terrain Profile Graph you would be able see the current standing with the terrain elevation.

<figure><img src="../../.gitbook/assets/Screenshot 2025-02-10 at 7.19.36 PM.png" alt=""><figcaption><p>Breakpoint preview during a grid mission</p></figcaption></figure>



## Warnings

If the planned altitude parameters for the mission exceeds limits or creates a conflict with the terrain, FlytBase provides an immediate warning, ensuring compliance with safety protocols.

{% hint style="warning" %}
Operators would be able to see an advance warning under the Terrain Profile Graph in case any point on the mission path would come in close contact with the ground (within 20 meters) when the mission is selected. In this case a review of the mission parameters is strongly recommended.
{% endhint %}

<figure><img src="../../.gitbook/assets/Untitled design-14-2.png" alt=""><figcaption><p>Warning for ground collision</p></figcaption></figure>

{% hint style="warning" %}
Operators would be able to see an advance warning over the Terrain Profile Graph in case any point on mission path exceeds the maximum altitude limit specified for the drone in device settings when the mission in selected. In this case a review of the mission parameters is recommended.
{% endhint %}

<figure><img src="../../.gitbook/assets/Untitled design-15-3.png" alt=""><figcaption><p>Warning for exceeding maximum limit </p></figcaption></figure>
