---
description: >-
  Learn more on how to configure collision avoidance sensing for your drone on
  the FlytBase dashboard.
---

# Collision Avoidance Sensing (CAS)

* Collision Avoidance Sensing enables your drone to detect obstacles in real-time.
* To configure this feature for your drone, navigate to the DJI Pilot 2 app, wherein you can toggle the "Obstacle Avoidance" feature and set the braking and warning distance for your drone. The drone will adhere to the RC's settings and automatically stop when an obstacle is detected within its braking distance.
* Your drone has two types of detection systems: the vision system and the infrared sensing system. These systems work together, allowing the drone to detect objects and stop at a set braking distance.

<figure><img src="../../../../.gitbook/assets/image (445).png" alt=""><figcaption><p>Detection Range of the Vision System (Source: DJI)</p></figcaption></figure>

<figure><img src="../../../../.gitbook/assets/image (446).png" alt=""><figcaption><p>Detection Range of the Infrared Sensing System (Source: DJI)</p></figcaption></figure>

{% hint style="info" %}
For more detailed information regarding the behavior of Obstacle Sensing, please consult the [DJI User Manual](https://dl.djicdn.com/downloads/m30_series_dock_bundle/UM/20230824/M30_Series_Dock_Bundle_User_Manual_v1.4_1EN.pdf), specifically on pages 39-47.
{% endhint %}

## Configuring Collision Avoidance Sensing for your Drone

<figure><img src="../../../../.gitbook/assets/RC Video (1).gif" alt=""><figcaption><p>Configuring Collision Avoidance Sensing for your Drone</p></figcaption></figure>

* Ensure that your Drone is powered "ON".
* Navigate to DJI Pilot 2 app on your RC Plus and bind the drone. (Ensure that RC Plus is selected as "Controller B")

<figure><img src="../../../../.gitbook/assets/image (489).png" alt=""><figcaption><p>Setting RC Plus as "Controller B"</p></figcaption></figure>

* Click on the "Enter Camera View" button.

<figure><img src="../../../../.gitbook/assets/image (455).png" alt=""><figcaption><p> DJI Pilot 2 app window</p></figcaption></figure>

* Navigate to "Obstacle sensing settings" by clicking on <img src="../../../../.gitbook/assets/image (448).png" alt="" data-size="line">button.

<figure><img src="../../../../.gitbook/assets/image (456).png" alt=""><figcaption></figcaption></figure>

<figure><img src="../../../../.gitbook/assets/image (457).png" alt=""><figcaption><p>Navigating to "Obstacle Sensing Settings"</p></figcaption></figure>

* Ensure that the Obstacle Avoidance toggle is set to "Brake," indicating that the obstacle avoidance feature for your drone is powered "ON."
* Configure the "Braking Distance" and "Warning Distance" for Horizontal, Vertical and Downward obstacle avoidance sensors.

{% hint style="info" %}
The warning distance must be set larger than the braking distance.
{% endhint %}

<figure><img src="../../../../.gitbook/assets/image (447).png" alt=""><figcaption><p>Configuring Braking and Warning Distance</p></figcaption></figure>

## Navigating to Collision Avoidance Sensing (CAS) on the FlytBase Dashboard

* Click on <img src="../../../../.gitbook/assets/image (452).png" alt="" data-size="line">button and navigate to "Device Management" tab.
* Select the device that you want to configure.
* Go to "Device Settings".
* Under this, you can see information related to Collision Avoidance Sensing (CAS) on the FlytBase dashboard.

<figure><img src="../../../../.gitbook/assets/capture_20240419191050553.bmp" alt=""><figcaption><p>CAS Information and Toggle button</p></figcaption></figure>

* While using manual controls, you would be able to see the navigation display showing nearby obstacles around the drone.

<figure><img src="../../../../.gitbook/assets/Nearby Obstacles_02-01.jpg" alt=""><figcaption><p>Navigation display showing nearby obstacles</p></figcaption></figure>

## Expected Behavior

| Scenario                                   | Description                         | Behaviour                                                                                                                                                                                         |
| ------------------------------------------ | ----------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| Drone is performing an autonomous mission. | It detects an obstacle on its path. | The drone will stop at the configured braking distance and hover. You can either take in manual controls to move around or perform RTDS.                                                          |
| Drone is performing RTDS                   | It detects an obstacle on its path. | The drone will stop at the configured braking distance and hover. You can take in manual controls to move the aircraft away.                                                                      |
| Drone is performing a manual mission.      | It detects an obstacle on its path. | You will be able to see nearby obstacles on the navigation display for enhanced situational awareness. The drone will stop at a configured braking distance and hover. You can then perform RTDS. |

<figure><img src="../../../../.gitbook/assets/image (490).png" alt=""><figcaption><p>Collision Avoidance Sensing (CAS) Navigation Display while using Manual Controls </p></figcaption></figure>

<figure><img src="../../../../.gitbook/assets/image (491).png" alt=""><figcaption><p>Collision Avoidance Sensing (CAS) Navigation Display in Cockpit View</p></figcaption></figure>
