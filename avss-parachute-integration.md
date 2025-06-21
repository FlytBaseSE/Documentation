# AVSS Parachute Integration

Overview

The AVSS Parachute Integration significantly enhances the safety of drone operations by providing emergency landing capabilities. This integration allows for real-time monitoring and control of the parachute system, ensuring swift and reliable deployment in critical situations.

​The AVSS Parachute Integration incorporates an **Autonomous Triggering System (ATS)** that continuously monitors the drone's flight parameters, including altitude, orientation, and acceleration. If the system detects anomalies indicative of a critical failure—such as rapid descent, loss of control, or other abnormal behaviors—it automatically initiates the parachute deployment sequence. This proactive approach ensures that the parachute is deployed promptly during emergencies, even without pilot intervention, thereby enhancing the safety and reliability of drone operations.

Within FlytBase workflows, this feature is essential for operators aiming to equip their flights with an emergency deployment option, thereby minimizing risks associated with unexpected flight failures. The integration aligns with regulatory standards such as ASTM F3322-22 and EASA MOC 2512, facilitating compliance for operations over populated areas and beyond visual line of sight (BVLOS).

{% hint style="info" %}
&#x20;This feature is currently compatible with the DJI Dock 2 and supports specific drone models, including the DJI M3D and M3TD.
{% endhint %}

## Key Features:

* **Automated and Manual Parachute Deployment:** The parachute system supports both automatic and manual deployment, activating upon detecting predefined emergency conditions, and manual deployment by operators on the FlytBase Operations Dashboard, allowing flexibility to handle various operational scenarios.
* **Real-time Parachute State Monitoring and Updates:** Continuous monitoring of the parachute system's status ensures operators are informed of its readiness and any potential issues.​
* **Secure Controls for Parachute Deployment with Visual Feedback:** Operators can manually deploy the parachute, with visual indicators confirming successful activation.​
* **Parachute Recovery System (PRS) + Flight Termination System (FTS):** The integrated PRS and FTS provide a comprehensive safety mechanism, enabling automatic deployment in less than 0.5 seconds and offering manual deployment options to meet various operational requirements.

{% hint style="info" %}
The Parachute Recovery System (PRS) is compatible with both the PRS-M3DTEX (EU variant) and PRS-M3DT (US variant). However, the Flight Termination System (FTS) is exclusively supported on the PRS-M3DTEX model of the AVSS Parachute. Following are the key differences between the EU and US variants:\


1. PRS-M3DTEX supports FTS, and whenever the parachute is deployed, the motors are stalled first, and then the drone gets powered off. For the PRS-M3DT variant, the drone motors are stalled, but the drone remains powered on.
2. Geofence management and breach-based automatic trigger parachute deployment is supported only for the PRS-M3DTEX.
{% endhint %}

## Steps to Manually Deploy the Parachute System

### Step 1: Access the Parachute Control

{% hint style="info" %}
**Note:** Ensure the drone is armed before attempting parachute deployment, as deployment controls are not available when the drone is disarmed.
{% endhint %}

* On the operations dashboard, click on the card of the drone which you wish to control.
* In the drone's detailed view, locate the 'Missions' control panel.
* Select the desired **path/grid mission** from the list or provide a **Go To Location (GTL)** command.
* Once the drone is armed, you would be able access the manual parachute deploy button.

### Step 2: Monitor Parachute Status

* Review the parachute status displayed on the drone control panel.
* Indicators will show whether the parachute is **armed**, **connected**, or in an **error state**.

{% hint style="danger" %}
**Warning:** Always visually confirm the parachute's readiness before initiating any flight operations.
{% endhint %}

<figure><img src=".gitbook/assets/Image 3-31-25 at 3.57 PM (1).jpeg" alt=""><figcaption></figcaption></figure>

### Step 3: Deploy the Parachute Manually (In Emergency Situations)

* Utilize the "Deploy Parachute" button.
* Press and hold the button for 3 seconds to activate the parachute deployment.
* Observe the progress visualization in the status window to confirm deployment.

<figure><img src=".gitbook/assets/Fleet view-15.png" alt=""><figcaption><p>Progress Visualization during Parachute Deployment</p></figcaption></figure>

### Step 4: Monitoring Post-Deployment Status

* Check for automatic system alerts indicating successful deployment.

<figure><img src=".gitbook/assets/Fleet view-17.png" alt=""><figcaption><p>System alert after Parachute Deployment</p></figcaption></figure>

* Verify that the drone status reflects the parachute's deployment and you would be able to see the last known location of the drone indicated by the coordinates on the map.

<figure><img src=".gitbook/assets/image (616).png" alt=""><figcaption><p>Last known location of Drone on Map</p></figcaption></figure>

* Once the drone is rescued confirm the Mark drone as rescued acknowledgement and then the map, alerts and launch panel with be reset to default.

<figure><img src=".gitbook/assets/Fleet view-18.png" alt=""><figcaption><p>Drone Rescue Acknowledgement</p></figcaption></figure>
