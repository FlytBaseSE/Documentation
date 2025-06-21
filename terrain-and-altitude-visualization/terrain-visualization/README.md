---
description: >-
  A guide to using the Terrain Visualization feature, which provides an estimate
  of the terrain features along your flight path, helping you plan and execute
  your flights safely.
---

# Terrain Visualization

## Overview

* The Terrain Visualization feature is a powerful tool designed to enhance flight safety and optimize mission planning. It provides operators with a clear view of the terrain along the drone’s flight path, highlighting key elevation changes and potential obstacles.&#x20;
* This feature allows operators to plan with confidence by visualizing altitude variations, waypoint elevations, and safe flight thresholds.&#x20;

## Terrain Profile Graph

The **Terrain Profile Graph** displays elevation changes along the planned flight path of the drone. This helps operators assess altitude variations during any particular flight. Following information is displayed as part of the Terrain Profile Graph:

* **Dock Altitude:** This is used as the reference for all altitudes displayed on the graph&#x20;
* **Waypoint Altitudes:** Height of each waypoint is displayed along the flight path
* **Go To Safe Altitude (GTSA): A**ltitude set for GTSA action is marked on the graph
* **Return to Docking Station (RTDS):** Altitude set for RTDS action is visible on the graph
* **Maximum Altitude Limit:** The upper limit of flight altitude is marked on the graph

{% hint style="info" %}
The **Terrain Profile Graph** uses these units on its axes:

* **X-axis:** **Distance** along the flight path (meters, feet, or yards)
* **Y-axis:** **Altitude** relative to the Dock (**Relative to Takeoff, RLT**) (meters, feet, or yards)
{% endhint %}

* The Terrain Profile Graph is available before executing Path, Grid and Waypoint Missions.&#x20;
* This allows users to have an extensive overview of the terrain along the mission path and also provides them caution and warning information before executing a mission.

<figure><img src="../../.gitbook/assets/Flight preview.png" alt="" width="563"><figcaption><p>Terrain Profile Graph preview before mission execution </p></figcaption></figure>

* The Terrain Visualization information is also available before performing Go To Location (GTL) flights.
* &#x20;Here operators will be able to choose between Above Ground Level (AGL) and Above Sea Level (ASL) as the reference altitude before setting the GTL parameters.

{% hint style="warning" %}
The terrain information regarding the possible NFZs on the flight path will not be reflected in the Terrain Profile Graph.
{% endhint %}

<figure><img src="../../.gitbook/assets/Frame 427322408.png" alt=""><figcaption><p>Terrain Profile Graph preview before giving Go To Location (GTL)  command</p></figcaption></figure>
