---
description: >-
  The Mission Breakpoint feature is designed to allow you to resume a mission
  from the last point of interruption. Here's a detailed guide on when and how
  to use it.
---

# Mission Breakpoint

### Mission Breakpoint

The Mission Breakpoint feature is designed to address interruptions during missions. These interruptions can result from technical, operational, environmental, or safety concerns.

### Common Causes of Mission Interruptions:

1. **Hardware Issues:** Malfunctions such as low battery, faulty GPS, rotor or propeller damage, or sensor failures.
2. **Communication Failures:** Signal disruptions between the drone and its docking station.
3. **Manual Intervention:** Operator overrides for perceived risks or manual maneuvers.
4. **Mission Planning Errors:** Misconfigured waypoints, altitude settings, or geofencing boundaries.
5. **Radio Frequency Interference (RFI):** Disruptions from nearby electronic devices or systems.
6. **Return to Docking Station (RTDS) Activation:** Triggered by low battery, signal loss, or safety thresholds.
7. **Fail-Safe Mode:** Automatic halting of missions due to activation of device fail-safes or weather conditions.

### Breakpoint Overview:

* A **Breakpoint** represents the exact progress of completion at which the drone aborts its mission due to a voluntary or involuntary event.&#x20;
* The Mission Breakpoint feature enables users to resume incomplete missions from the last achieved point rather than restarting from the beginning. Resumption are based on the type of mission:
  * **Path Mission:** Resumes from the last waypoint reached before the interruption.
  * **Grid Mission:** Resumes from the last sharp angle covered during the previous flight.

### Using the Breakpoint Feature:

1. **Execute a Mission:** Start a pre-planned mission from the **Drone Control Panel**. [Refer the FlytBase Flight Execution section to execute a pre-planned mission.](../../../in-flight-modules/flight-execution/#how-to-execute-a-pre-planned-mission)

<figure><img src="../../../.gitbook/assets/Screenshot 2024-12-27 191058 (1).png" alt=""><figcaption><p>Executing a pre-planned Mission</p></figcaption></figure>

2. **Abort Mission:** Click the **RTDS** (Return to Docking Station) button on the drone control panel to safely abort and return the drone to the dock.

<figure><img src="../../../.gitbook/assets/Screenshot 2024-12-27 191415.png" alt=""><figcaption><p>Using the RTDS command to abort a live mission</p></figcaption></figure>

3. **Access Saved Missions:**&#x20;
   * Navigate to the **Mission** tab in the drone control panel. The **Mission** tab will display a small blue dot indicating that there are some incomplete missions.
   * &#x20;Incomplete missions are indicated with the label **Incomplete** and display relevant details such as the percentage of mission left and estimated completion time.&#x20;
4. **Resume Mission:**
   * Select the desired incomplete mission and then click 'Resume'
   * Confirm the safety checklist parameters and click 'Launch'

<figure><img src="../../../.gitbook/assets/Screenshot 2024-12-27 191645 (1).png" alt=""><figcaption><p>Resuming incomplete missions from the operations dashboard</p></figcaption></figure>

5. **Completion:** The drone will restart from the designated Breakpoint:

* For Path Missions: The mission resumes from the last waypoint reached before the interruption.

<figure><img src="../../../.gitbook/assets/Screenshot 2024-12-27 191925 (1).png" alt=""><figcaption><p>Drone resuming the incomplete Path mission </p></figcaption></figure>

* For Grid Missions: The mission esumes from the last sharp angle covered during the previous flight.

<figure><img src="../../../.gitbook/assets/Screenshot 2024-12-27 194004 (1).png" alt=""><figcaption><p>Drone resuming the incomplete Grid mission </p></figcaption></figure>

{% hint style="info" %}
You can restart any incomplete mission by clicking the **Reset** button next to it in the **Missions Tab** of the **Drone Control Panel**.
{% endhint %}

### Scenarios Where Breakpoint Can Be Used:

* Mission aborted due to technical, operational, or environmental issues.
* Missions interrupted by manual **RTDS** action.
* Manual intervention using the **STOP** button followed by the RTDS command.

### Scenarios Where Breakpoint Cannot Be Used:

* Deleted missions.
* Mission where the mission parameters have been modified.
* Missions that are aborted before the drone reaches the first waypoint.
* Missions reset via the Operations Dashboard.

### Resuming Missions Mid-Air:

If the mission is stopped mid-flight for **manual control** or a **Go-To-Location (GTL)** command, it can still be resumed from the last waypoint.

{% hint style="info" %}
If **RTDS** is initiated, resumption is only possible after the drone returns to the dock.
{% endhint %}
