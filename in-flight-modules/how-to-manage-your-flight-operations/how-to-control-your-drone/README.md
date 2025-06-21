---
description: >-
  Learn how to control essential drone functions such as Return to Docking
  Station, Pause, Resume, and Abort functionalities.
---

# How to Control Your Drone

## Drone Control Panel  Overview

The Drone Control Panel serves as a centralized hub, offering operators crucial flight information and commands, making essential drone tasks easily accessible at your fingertips. It is located in the bottom-center region of the dashboard.

<figure><img src="../../../.gitbook/assets/image (154).png" alt=""><figcaption><p>Drone Control Panel on FlytBase Dashboard</p></figcaption></figure>

### View In-flight Information

<figure><img src="../../../.gitbook/assets/image (161).png" alt=""><figcaption><p>In-flight Information</p></figcaption></figure>

The Drone Control Panel provides the operator with access to view the following in-flight information of the drone:&#x20;

1. Mission Status Indicator - Shows the real-time mission completion percentage.&#x20;
2. Drone State <img src="../../../.gitbook/assets/image (162).png" alt="" data-size="line">- Indicates the real-time status of the drone. Following are the different states represented by the drone.
   1. In-flight - This state indicates that the drone is performing a mission or executing a 'Go to location' command.
   2. Hovering - This state means the drone is currently hovering in place.
   3. Offline - This state indicates that the drone is currently offline.
3. Mission Name - Provides info regarding the pre-planned mission being executed.

### Drone Control Commands

Operators can use the drone control panel to execute the following commands:

* Return To Docking Station (RTDS) <img src="../../../.gitbook/assets/image (107).png" alt="" data-size="line">- Directs the aircraft back to the docking station.
* Pause <img src="../../../.gitbook/assets/image (106).png" alt="" data-size="line">- Pauses aircraft's motion and makes it enter into a hover standstill.
* Resume <img src="../../../.gitbook/assets/image (292).png" alt="" data-size="line"> - Continue planned aircraft activities initiated before the 'Pause' command.
* Abort <img src="../../../.gitbook/assets/image (158).png" alt="" data-size="line">- Stops all active drone commands and makes it hover in place instantly.

{% hint style="success" %}
Resume button will only be available when the drone is performing a mission.
{% endhint %}

{% hint style="danger" %}
Note that the Pause option is only supported when the drone is performing a pre-planned mission.
{% endhint %}

{% tabs %}
{% tab title="Return to Docking Station (RTDS)" %}
### Return to Docking Station (RTDS)

This function brings the aircraft back to the docking station. The functionalities of the Return to Docking Station (RTDS) feature are as follows:

* When the finish action is set to RTDS during mission planning, it automatically triggers Return to docking station (RTDS) upon mission completion.
* RTDS automatically engages during a DJI failsafe event.
* You can manually engage RTDS during an ongoing mission.
* When launching to a location, you can activate RTDS only after engaging the 'Abort' button.

#### Steps to use Return to Docking Station (RTDS):

1. During a mission or Go to location, operators can command RTDS from the drone control panel.

<figure><img src="../../../.gitbook/assets/image (153).png" alt=""><figcaption><p>RTDS button</p></figcaption></figure>

2. Upon pressing the button, the operator would receive a confirmation pop-up following which toaster messages (notifications) would appear on the dashboard and the drone starts executing RTDS (Return to Docking Station) command.

<figure><img src="../../../.gitbook/assets/image (111).png" alt=""><figcaption><p>Confirmation message while executing RTDS for the drone</p></figcaption></figure>
{% endtab %}

{% tab title="Pause" %}
### Pause

This function is used to pause the movement of aircraft while it is executing any command. When activated, the drone swiftly transitions into a standstill mode, hovering in place.

The functionalities of the 'Pause' button are as follows:

* The Pause button is only usable during a planned mission.
* It cannot be used when the drone is performing a Go-to location.

{% hint style="info" %}
To interrupt a Go to location mission, utilize the 'Abort' option, as pausing is not available for this type of mission.
{% endhint %}

#### Steps to use the Pause function:

1. While the drone is undertaking a mission, the operator can click on 'Pause' button located on the drone control panel.

<figure><img src="../../../.gitbook/assets/image (144).png" alt=""><figcaption><p>'Pause' button</p></figcaption></figure>

2. Upon pressing the button, the operator would receive a confirmation on the dashboard in the form of toaster messages (notifications).

<figure><img src="../../../.gitbook/assets/image (147).png" alt=""><figcaption><p>Toaster message upon pressing 'Pause' button</p></figcaption></figure>

3. The drone starts hovering, and the drone state is displayed as 'Paused' on the drone control panel.

<figure><img src="../../../.gitbook/assets/image (146).png" alt=""><figcaption><p>Drone State upon executing 'Pause' button</p></figcaption></figure>
{% endtab %}

{% tab title="Resume" %}
### Resume

This function resumes planned aircraft activities that were initiated before issuing a 'Pause' command.

The functionalities of the 'Resume' button are as follows:

* Activating 'Resume' during a preplanned mission after using 'Pause' directs the drone to resume executing the mission commands from the point where the mission was paused.
* You cannot use 'Resume' when 'Abort' is engaged during a Go-to location. Instead, you have the option to perform RTDS or set another Go-to location.

#### Steps to use the Resume function:

1. Once 'Pause' is engaged in a preplanned mission, the same button transforms into a 'Resume' button, situated on the drone control panel on the FlytBase dashboard.

<figure><img src="../../../.gitbook/assets/image (149).png" alt=""><figcaption><p>Resume button</p></figcaption></figure>

2. Press the button to receive a pre-flight checklist.

<figure><img src="../../../.gitbook/assets/image (150).png" alt=""><figcaption><p>Pre-flight checklist</p></figcaption></figure>

3. Check all safety [checklist](../../../pre-flight-modules/platform-settings/checklist.md) parameters. Once confirmed, a dashboard message will pop up, and the drone will continue executing commands from where it was paused.

<figure><img src="../../../.gitbook/assets/image (151).png" alt=""><figcaption><p>Toaster message upon pressing ' button</p></figcaption></figure>
{% endtab %}

{% tab title="Abort " %}
### Abort Function Overview

The 'Abort' function serves as a quick and immediate stop for the drone. When activated, the drone swiftly transitions into a standstill mode, hovering in place. This allows for precise control and safety during drone operations.&#x20;

The abort function can only be used in the following scenarios:

<table><thead><tr><th width="197">Scenario</th><th>Expected Behavior </th></tr></thead><tbody><tr><td>When the drone is performing Go-to Location</td><td><ol><li>Once the Operator engages the 'Abort' button, the drone will abort its current action and hover at its location. </li><li>The drone instantaneously enters a standstill mode,  hovering in place refusing any additional commands from the dashboard, and can only perform RTDS when triggered by you. </li></ol></td></tr><tr><td>During 'GO_HOME' commands like Return to Docking Station (RTDS) or DJI failsafe triggers</td><td><ol><li>Once the Operator engages the 'Abort' button during 'GO_HOME' commands, such as Return to Docking Station (RTDS) or DJI failsafe triggers, the drone will abort its current action and hover at its location.</li><li>It will remain in this state until the Resume action is initiated from the dashboard. </li></ol></td></tr></tbody></table>

<figure><img src="../../../.gitbook/assets/image (156).png" alt=""><figcaption><p>'Abort' button during GO_HOME</p></figcaption></figure>

This safety measure ensures that when the drone is executing 'Go-to location' and 'GO\_HOME' commands, it avoids potential emergencies head-on, enabling operators to swiftly intervene and prevent unintended movements right from the dashboard.

**Steps to use the 'Abort' feature:**&#x20;

1. While the drone executes a 'Go-to location' or 'GO\_HOME' command, operators can take swift action by clicking the 'Abort' button located on the drone control panel.

<figure><img src="../../../.gitbook/assets/image (157).png" alt=""><figcaption><p>'Abort' button on drone control panel.</p></figcaption></figure>

2. Upon pressing the button, the operator would receive a confirmation on the dashboard in the form of toaster messages (notifications).
{% endtab %}
{% endtabs %}
