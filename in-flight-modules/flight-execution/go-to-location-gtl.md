---
description: A guide for quickly launching the drone to a specific location.
---

# Go to Location (GTL)

The **Go-to Location (GTL)** feature enables a drone to fly to a specified GPS point autonomously. Users can mark the location on the FlytBase Dashboard, and the drone will navigate there and hover. Once at the location, the drone can be manually controlled to perform desired actions.

{% hint style="info" %}
The **Go to Location** feature can be used even when the drone is powered off. The drone will automatically power on once the Go-to Location command is initiated.
{% endhint %}

## Initiating a Go to Location (GTL) flight

* Click on ![](<../../.gitbook/assets/Hamburger Menu.svg>) and select **Fleet**
* Select the desired drone from the list of available drones.
* On the **Drone Control Panel,** select <img src="../../.gitbook/assets/GTL.svg" alt="" data-size="line">.
* A configuration window will appear, enabling you to select a location on the map and adjust the flight settings accordingly.
  * Click on the map to drop a pin at the desired location.
  * Adjust the mission settings as needed to ensure the drone follows a safe flight path and avoids obstacles.
* Click on **Launch**
* Complete the pre-flight checklist and click on **Execute**

{% embed url="https://youtu.be/Ytxh5SSIrVs" %}
\[Video] Initiating a Go to Location flight
{% endembed %}



## Flight Parameters for Go to Location

1. **Latitude and Longitude** values for the Waypoint.
   * Click on the map to drop a pin at the desired location.
2. **Task Altitude:** This parameter defines a dedicated cruising height between takeoff and Go To Location (GTL) destination, providing enhanced obstacle clearance and flight path control during flights.
   * Task Altitude only affects your drone's path when it would otherwise fly below this height. If your drone is already above Task Altitude, it will maintain its current height.
   * The drone will ascend to the higher of either Safe Takeoff Altitude or Task Altitude when beginning a Go To Location.
   * Task Altitude changes during flight only affect subsequent Go To Location commands, not the current flight path.
   * After a Go To Safe Altitude event, Task Altitude may be temporarily modified to GTSA height. You'll see an indicator and option to restore previous settings.
   * This parameter can be predefined in the Device Settings page for configuring default values that persist across flights.

<figure><img src="../../.gitbook/assets/Image 5-27-25 at 5.55 PM.jpeg" alt=""><figcaption><p>Task Altitude Settings </p></figcaption></figure>

<table><thead><tr><th width="144">Your Settings</th><th width="283">Drone Behavior</th><th>When to Use This</th></tr></thead><tbody><tr><td>Task Altitude is highest</td><td>The drone climbs straight up to Task Altitude, flies level to the destination maintaining this height, then drops straight down to the final landing altitude. This creates a clear separation between climb, cruise, and descent phases.</td><td><strong>Flying over obstacles or terrain</strong> - Perfect for crossing forests, buildings, or hills where you need guaranteed clearance throughout the entire flight path.</td></tr><tr><td>Safe Altitude is highest</td><td>The drone first climbs to Safe Altitude for immediate takeoff safety, then adjusts down to Task Altitude for efficient travel, and finally descends to the destination altitude. This provides a balanced approach between safety and fuel efficiency.</td><td><strong>Standard missions</strong> - Good balance of safety and efficiency for most routine operations where you need initial takeoff clearance but don't require maximum cruise altitude.</td></tr><tr><td>Waypoint Altitude is highest</td><td>The drone climbs gradually while flying forward in a diagonal path directly to the destination. Task Altitude is effectively ignored since it would be lower than both current and target altitudes, making the flight as efficient as possible.</td><td><strong>Flying uphill to higher destinations</strong> - Most efficient when your destination is at a higher elevation than your takeoff point, such as flying from ground level to a rooftop or hilltop.</td></tr></tbody></table>

{% hint style="info" %}
**Visualization Enhancements**: The Terrain Profile Graph includes a visual representation of the Task Altitude, helping you plan and visualize your complete flight path before execution.
{% endhint %}

{% hint style="warning" %}
**Compatibility**: This feature is compatible with all currently supported DJI docks. Task Altitude is not supported for legacy GTL operations.
{% endhint %}

3. **Safe Altitude:** This setting specifies the altitude the drone will reach after take-off. Once at this altitude, the drone will proceed to the Waypoint.&#x20;

* If the Waypoint Altitude is higher than the Safe Altitude, the drone will fly diagonally toward the Waypoint.
* The drone’s approach to a Waypoint at a lower altitude than the Safe Altitude may vary based on ambient lighting conditions.

<figure><img src="../../.gitbook/assets/Safe Altitude GTL.jpg" alt="" width="523"><figcaption><p>Alternative approaches to a Waypoint lower than Safe Altitude</p></figcaption></figure>

4. **Waypoint Altitude:** This is the altitude the drone will maintain when it reaches the specified coordinates of the Waypoint.

{% hint style="info" %}
&#x20;You can set the Take-Off Altitude to be the same as the Waypoint Altitude.
{% endhint %}

5. **Drone Speed, Finish Action, and Total Distance to Cover:** These parameters cannot be altered, but their presence in configuration window provides information necessary to complete the Go to Location flight.

{% hint style="warning" %}
You cannot adjust the drone's speed during the 'Go to Location' operation. The drone will gradually reach a velocity of 15 m/s over the specified distance.
{% endhint %}

6. Click **Launch** to send the drone to the specified location.

<figure><img src="../../.gitbook/assets/GTL Config window.jpg" alt="" width="282"><figcaption><p>Go to Location configuration window</p></figcaption></figure>

{% hint style="info" %}
You can also use the **Go to Location** function to launch the drone to a specific location during a mission. You can do this by:&#x20;

* **STOP** the current mission for the desired drone
* Click on <img src="../../.gitbook/assets/GTL.svg" alt="" data-size="line"> in **Drone Control Panel**
* Mark the location on the map
* Configure flight settings&#x20;
* Click on **Launch** and clear the pre-flight checklist
{% endhint %}

## Expected Behavior of Drone during Go to Location

* The drone will ascend to the highest of Safe Altitude or Task Altitude relative to the docking station.
* The drone will then move towards the specified Waypoint coordinates, slowly achieving a top speed of 15 m/s, and adjusting its altitude according to the Task Altitude configuration.
* The drone starts hovering upon reaching the desired location.

{% hint style="info" %}
While the drone is en route to the marked location, you can pause the Go to Location action at any time using the **STOP** button on the FlytBase Dashboard.
{% endhint %}
