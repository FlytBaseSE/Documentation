# Real-Time Fleet Monitoring

## Drone Status Tracking

Status indicators showing whether docks are Online, Offline, or Armed with color-coded visual indicators:

* Green: Dock is operational and ready
* Orange: Dock is armed or in transition state
* Grey: Dock is offline or experiencing issues

<div align="center"><figure><img src="https://lh7-rt.googleusercontent.com/docsz/AD_4nXcPg0KSuTZsd6POa-gvqZmPOypMDjmX9G2oCMlwKogqZoOA2oen7TJEr4g24eolIpxSkdFVpOXlPIUSAQ5jIhC-3CriJeIxg8jELVuQwQwy1PaolnQGAjiB7kpFcOGF6auIVPynjw?key=ltwtiAhGhp6bUzvxpSYaXw" alt="" width="188"><figcaption><p>Drone Status Tracking</p></figcaption></figure></div>

## Operations Data Visibility&#x20;

<figure><img src="https://lh7-rt.googleusercontent.com/docsz/AD_4nXcx6U9PxBw6YuJ5dNMvqZEIgZGZxu2XqLO4Kqvn-EE0CHoR68jrjH6FDmcaTslWQWTijZqOWVPTnXRz4qYASNzH916EN9hyFJ8zfNHTY_EY_DgRMSa-52p0SW_BkCKXzu7o7IYH?key=ltwtiAhGhp6bUzvxpSYaXw" alt=""><figcaption><p> Operations Data Visibility table showing operations data with multiple drones across different sites</p></figcaption></figure>

Monitor essential flight parameters including:

* Name: Unique drone name as an identifier for fleet tracking
* RLT/AGL: Indicates the drone's altitude relative to the docking station or the ground level. If a Digital Terrain Model (DTM) is imported, the altitude values will be adjusted accordingly based on the DTM data.
* Operation: Current mission or operational task being performed ( Mission or Standby)
* System state: Current operational status (RTDS, Hovering, Landing & In Progress)
* Command status: Provides a comprehensive view of all commands with real-time status updates and detailed timestamps. Commands transition from "In Progress" to "Completed" upon successful execution, offering immediate feedback. Any failed commands are clearly flagged, enabling quick retries or alternative actions for seamless operational control.
* Health: Device health indicators with critical errors and warning messages, displaying detailed error codes for comprehensive diagnostics.
* Airspace: Comprehensive environmental alerts system monitoring both airspace threats and weather conditions that could impact drone operations, providing real-time safety awareness for Beyond Visual Line of Sight (BVLOS) compliance.
*   Airspace Threat Detection:

    * Automatic real-time detection and notification of airspace conflicts
    * Detailed threat information: Unique threat IDs, ICAO codes, and precise altitude parameters
    * Severity classification: Critical (red) and warning (yellow) level categorization
    * Multiple threat tracking: Monitor up to 6 simultaneous threats per drone with altitude conflict zones.



    <figure><img src="https://lh7-rt.googleusercontent.com/docsz/AD_4nXdg6z4wUBJCoBnyY-H8Gw5ZvLhbAnAc6ggJNW50UlPQzXYNbUnDCLdLWEL6_qWmHpv5DnoZPxNFNHpfJjYIG-QPx0ciDIgMF-L1f7m6s9x-FO8fQ1bhO01kPWNbj29KTLN_KpBW6w?key=ltwtiAhGhp6bUzvxpSYaXw" alt="" width="375"><figcaption><p>Airspace Threats in action</p></figcaption></figure>
*   Weather Alerts:

    * Live weather monitoring: Real-time weather condition alerts affecting flight operations
    * Critical weather alerts: Immediate notifications for conditions like heavy rainfall requiring operational attention
    * Warning conditions: Alerts for moderate conditions such as wind speed changes that may impact missions
    * Timestamp tracking: Precise timing of all environmental events for operational planning



    <figure><img src="https://lh7-rt.googleusercontent.com/docsz/AD_4nXfNNncWtlIcgPKXrcJReS5D5-TolvG1Oe9qRd9Sy7iKhr-NGnr-tgozCZykAYigaLwK9t7H2tX9NnU_RvYSNLt8q30risp7ZBYq1DiMwEQqcRXvAxZR9lXP5bleQxxn2Mxk8xYejg?key=ltwtiAhGhp6bUzvxpSYaXw" alt="" width="375"><figcaption><p>Weather alerts in action</p></figcaption></figure>


* Actions: Quick access controls for individual drone management including view drone details, take control, center map view, and pin to dashboard.

## Controlling Drone Visibility

Every drone in your fleet can be individually shown or hidden using the eye icon controls. When you're managing operations across multiple sites, this becomes incredibly powerful for focusing on specific missions or geographic areas. To show or hide specific drones:

1. Select multiple drones: Use the checkboxes to select multiple hidden drones from your fleet.
2. Click the "Show" button: Located at the bottom of the interface, this instantly brings all selected drones into your active workspace.

<figure><img src="../../../.gitbook/assets/Image 28-05-25 at 7.45 PM.jpeg" alt="" width="375"><figcaption><p>Controlling drone visiblilty </p></figcaption></figure>

3. Monitor your selection: Watch the "Visible" counter update as you adjust your workspace.

<figure><img src="../../../.gitbook/assets/Image 28-05-25 at 7.49 PM.jpeg" alt="" width="375"><figcaption><p>Setting Drone to Visible Mode </p></figcaption></figure>

## Understanding Batch Operations

* Once you've optimized your operational visibility, Fleet View 2.0's bulk control capabilities transform time-consuming individual drone management into efficient fleet-wide operations. This addresses one of the most critical challenges in large-scale drone deployments: the need to coordinate safety commands or emergency responses across multiple drones within seconds rather than minutes.
* Batch operations are Fleet View 2.0's superpower for simultaneous multi-drone control. Instead of manually commanding each drone individually – which could take minutes during critical situations – batch operations let you execute the same command across multiple drones with a single action.
* The following commands currently supported in batch operations:
  * Take Control: This changes the pilot in control for the selected drones.
  * Go To Safe Altitude: Selected drones to immediately ascend to predetermined safe altitude levels for conflict avoidance.
  * Return to Docking Station: Initiates automated return sequences for selected drones, sending them back to their assigned docking stations.
  * Stop: Immediately halts all activities for selected drones, providing instant fleet-wide emergency response capability.

<figure><img src="https://lh7-rt.googleusercontent.com/docsz/AD_4nXev_VrwPuHntKyDW4kOb1i_1YgBN6prMkeCI1cbKym_xhlAObnnvs5roWke9SPUdMQRV2HaCGUZJyLebaU75SrdJvB8iHKo6HwLhN72mUe9LUPHV8Cc45qhB6aQzQ3nHcMZXiyNpA?key=ltwtiAhGhp6bUzvxpSYaXw" alt=""><figcaption><p>Commands available in Batch Operations</p></figcaption></figure>

{% hint style="info" %}
You can run batch operations (RTDS, GTSA, or STOP) on hidden drones—as long as they're online. Just select the checkbox next to any online drone in the Hidden section, choose your command, and execute. The drone will instantly become visible in your workspace with its video feed shown, so you can monitor the action right away.
{% endhint %}

## **Understanding the Pin Feature**

The **Pin** feature enables operators to prioritize specific drones for focused monitoring and tracking, ensuring continuous visibility of critical assets regardless of other ongoing operations. Pinning works across multiple sites and operational zones, allowing you to maintain focus on critical assets regardless of their geographic location. When a drone is pinned in **Fleet View 2.0**, the view dynamically adapts to enhance situational awareness around that asset by:

* **Prominent Video Display:** The drone’s video feed is centrally highlighted for maximum visibility. Additionally all associated video feeds—including payload and docking station cameras—are displayed.
* **Automatic Map Tracking:** The map view automatically follows the drone’s movement throughout its mission.
* **Priority Positioning:** Pinned drones are listed under a dedicated "Pinned" section at the top of your drone list for easy access.

### Pinning a Drone:

1. Click on the pin icon: Find the pin icon in the Actions column next to any drone.
2. Verify pinned status: The drone immediately moves to the "Pinned" section at the top of your list.
3. Monitor activation: Watch as Payload and FPV video feeds activate and the map centers on your pinned drone

<figure><img src="../../../.gitbook/assets/Image 28-05-25 at 6.46 PM.jpeg" alt=""><figcaption><p>Pinned Drone in View</p></figcaption></figure>

### Managing Pinned Drones:

1. Track pinned assets: Pinned drones appear under the dedicated "Pinned" header for instant identification.
2. Unpin when complete: Click the pin icon again to remove the drone from priority view and return to standard monitoring.
