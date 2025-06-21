---
description: >-
  Keywords - Failsafe Events, Failsafe Actions, Low Battery, Critical Battery,
  Link Loss
---

# Settings - Failsafes

## Overview

Failsafe events are unexpected emergencies, such as loss of communication, low battery, or inclement weather, that require immediate, predefined actions to ensure drone safety. Setting up failsafe responses is crucial for the safe and predictable operation of autonomous drones to minimize risks and prevent accidents or damage.

FlytBase allows you to configure these actions as part of Device Settings. By defining these failsafe actions in advance, you ensure that your drone can handle emergencies and maintain safety and reliability during autonomous operations.

<figure><img src="../../../.gitbook/assets/image (593).png" alt=""><figcaption><p>Failsafes on FlytBase</p></figcaption></figure>

## Failsafe Actions and Expected Behavior

When an emergency occurs that necessitates failsafe actions, the drone will execute one of the preset responses based on the configured failsafe actions.

<table><thead><tr><th width="310">Failsafe Action</th><th>Behavior when Action is executed</th></tr></thead><tbody><tr><td>Return To Docking Station (RTDS)</td><td>The drone will fly towards the Docking Station at a fixed speed and altitude. It will land on the Docking Station once it reaches the correct location.</td></tr><tr><td>Return to Safe Location (RTSL)</td><td>The drone will proceed to the marked Safe Location and land.</td></tr><tr><td>Hover</td><td>The drone will hover in place, and the user must take manual control from the FlytBase Dashboard or a secondary RC.</td></tr><tr><td>Land</td><td>The drone will land at its current location.</td></tr><tr><td>No Action</td><td>The drone will continue with its mission.</td></tr></tbody></table>

## Failsafe Settings

To configure Failsafe Settings for any particular device, follow these steps:

* Navigate to **Devices** -> _Select your device_ -> **Settings**, and select **Failsafe**.
* For each Failsafe event, set the Trigger value in the suggested range and a Failsafe Action.
* You can reset all fields by scrolling down the list and clicking on **Reset.**

## Failsafe Events and Actions

<table data-full-width="false"><thead><tr><th width="173" align="center">Failsafe Event</th><th width="207" align="center">Event Description</th><th width="165" align="center">Available Actions</th><th align="center">Recommended Action</th></tr></thead><tbody><tr><td align="center"><strong>Low Battery</strong></td><td align="center">A low battery level is indicated when the drone's remaining power reserve is enough to return to its Dock and land. The threshold for this event can be set in the range of 20%-50%.<br></td><td align="center"><p>RTDS</p><p>RTSL<br>Land<br></p></td><td align="center">RTDS or RTSL</td></tr><tr><td align="center"><strong>Critical Battery</strong></td><td align="center">A critical battery level is indicated when the drone's remaining power reserve is enough only to descend from the current altitude and land at the current location. The threshold for this event can be set in the range of 10%-15%.</td><td align="center">Land</td><td align="center">Land</td></tr><tr><td align="center">High Wind Speed</td><td align="center">The drone or the weather station on the Dock can detect wind speeds above a set threshold, which may endanger flight operations. In this case, flight operations must stop and the drone must return.</td><td align="center">RTDS<br>RTSL<br>No Action</td><td align="center">RTDS</td></tr><tr><td align="center">Heavy Rainfall</td><td align="center"> Excessive rainfall can damage the drone. To prevent such an event, the rainfall sensor on the weather station detects rainfall above the set threshold and sends a command to stop flight operations if needed.</td><td align="center">RTDS<br>RTSL<br>No Action</td><td align="center">RTDS</td></tr><tr><td align="center">Drone LTE Link Loss</td><td align="center">The Drone and Dock experience LTE Link Loss when the Dock is unable to communicate with the Cloud due to network interruptions. You can set a wait time before the failsafe action is triggered.</td><td align="center"><p>RTDS</p><p>RTSL<br>Hover<br>No Action</p></td><td align="center">RTSL<br><br><strong>Note:</strong> enabling Prioritize Mission means the drone would continue with its mission if RC Link is working.<br></td></tr><tr><td align="center">RC Link Loss</td><td align="center">RC Link Loss occurs when the RF connection (including 4G LTE) between the drone and Dock is lost. You can set a wait time before the failsafe action is triggered.</td><td align="center"><p></p><p>RTSL</p><p>Hover<br>Land</p></td><td align="center">RTSL</td></tr><tr><td align="center">GCS Link Loss</td><td align="center">GCS Link Loss happens when the user closes the FlytBase Dashboard or has poor network connectivity with the Cloud while the drone is active (ready-to-fly or in-flight). You can set a wait time before the failsafe action is triggered.</td><td align="center"><p>RTDS</p><p>RTSL<br>Land<br>Hover<br>No Action</p></td><td align="center">RTSL</td></tr><tr><td align="center">Precision Landing Timeout</td><td align="center">During Precision Landing, the drone hovers over the landing zone for a set time and tries to locate the landing tag. If it can't find the tag or stay in position, the Precision Landing operation ends, and an alternative landing process starts.</td><td align="center">RTSL</td><td align="center">RTSL</td></tr></tbody></table>

{% hint style="danger" %}
The safe landing location should be set for each device, and the safe landing location should be clear of any obstruction that can prevent safe landing.
{% endhint %}
