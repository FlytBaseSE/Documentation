---
description: >-
  A checklist of what is required to be ensured before a flight with the new
  Hextronics Atlas/Hextronics Universal. You must follow all the steps mentioned
  below for operating seamless flights.
---

# First Flight with Hextronics Atlas/Hextronics Universal

### Assigning a Site:

Before you begin your operations, you must add your devices to a site to ensure it is being operated by designated team members.

You can refer to the [Site Management](../../../getting-started-with-your-flytbase-account/site-management.md) document to learn more.

<figure><img src="../../../.gitbook/assets/image (2).png" alt=""><figcaption><p>Site Management</p></figcaption></figure>

### Marking the Docking Station Location and Safe Location:

In order to ensure that your Drone successfully initiates RTDS (Return To Docking Station) and RTSL (Return To Safe Location), you need to mark the respective locations on FlytBase.&#x20;

Refer to [this](settings-drone-and-dock.md#location) document to configure your landing locations.

<figure><img src="../../../.gitbook/assets/image (585).png" alt=""><figcaption><p>Landing Locations</p></figcaption></figure>

### Configure Precision Landing:

Precision Landing is a capability that allows drones to land precisely on designated Docking Stations.

FlytBase can be configured for two types of Precision Landing: Vision or RTK.

To learn more about configuring Precision Landing, refer to [this document](settings-precision-landing.md).

<figure><img src="../../../.gitbook/assets/image (586).png" alt=""><figcaption><p>Configuring Precision Landing</p></figcaption></figure>

### Updating Failsafes:

Now that the drones have a new 'home' to go to after completing a flight (i.e., the Docking Station), the operator can set appropriate safety actions, such as Return to Docking Station (RTDS) and Returning to Safe Location (RTSL), Land during events such as a low battery or network connectivity loss.

Refer to [this document](settings-failsafes.md) to learn more about failsafes and setting them as per your Operating Procedures.

<figure><img src="../../../.gitbook/assets/image (587).png" alt=""><figcaption><p>Failsafes</p></figcaption></figure>

### Enable Automate Operations:

In order to make sure that the Docking Station's commands are synced and automated with your drone for complete autonomous operations, you must enable Automated Operations from the Dock settings.

Refer to [Device Management documentation](broken-reference) to know more about this functionality.

Ensure that the Drone Control settings are also configured.

<figure><img src="../../../.gitbook/assets/image (588).png" alt=""><figcaption><p>Enable Automated Operations</p></figcaption></figure>

### Assigning a Geofence for your device:

Geofence is a virtual boundary for your drone that ensures your operations are confined within set geographical limits.

To create and assign a Geofence, refer to this[ link](first-flight-with-hextronics-atlas-hextronics-universal.md#assigning-a-geofence-for-your-device).

<figure><img src="../../../.gitbook/assets/image (589).png" alt=""><figcaption><p>Assigning a Geofence</p></figcaption></figure>

### Executing your first mission:

With all settings configured for flight, the operator is now ready to plan the mission. To do this, follow the steps described in [Creating a Mission section](../../../pre-flight-modules/planning/mission-planning/).

And to schedule, this mission at recurring intervals, the [Mission Scheduler ](../../../pre-flight-modules/planning/mission-scheduler.md)section can help in doing so.

### Post Flight:

After a successful run during the first flight using FlytBase, you can navigate to Flight Logs and check the flight details, and download the captured media (if any).\


<figure><img src="../../../.gitbook/assets/image (584).png" alt=""><figcaption><p>Flight Logs</p></figcaption></figure>

