---
description: Keywords- Flows, Automation, Workflows, Response
---

# Flows

**Flows** in FlytBase is a dynamic feature designed to streamline operational efficiency by configuring the drone's response to specific alarm triggers or operational notifications. These workflows allow for the deployment of drones in response to various alarm sources, with the option for missions to be approved manually or carried out automatically for repetitive events. They also allow selected organisation members to keep track of the drone operations by staying notified through emails or SMS.&#x20;

This capability empowers the integrated **Flinks** and significantly enhances responsiveness in sectors such as emergency response, security, and infrastructure monitoring, by reducing response times and the need for constant human intervention.&#x20;

## Setting up Flows

**Accessing the Flows Manager:**

* Select **Flows** from the Navigation Drawer to open the **Flows** section.

<figure><img src="../../.gitbook/assets/Untitled design (11) (2).png" alt=""><figcaption><p>Flows tab in Navigation Drawer</p></figcaption></figure>

**Flows Section Tabs:**

* **My Flows**: Here you can create, edit, and delete your flows. You can also enable and disable them when required.
* &#x20;**Logs**: This tab records the trigger time and status of each flow.

<figure><img src="../../.gitbook/assets/Image 18-02-25 at 8.30 PM.jpeg" alt=""><figcaption><p>Flows Manager</p></figcaption></figure>

## Creating a new Flow

To create a new Flow, please follow the following steps:

* In the **My Automations** tab, click on the **Create** button.
* A dialog box will appear, prompting you to select a category.&#x20;

{% hint style="info" %}
Currently only Alarms and Notifications based flows are supported.
{% endhint %}

<figure><img src="../../.gitbook/assets/Image 20-02-25 at 11.13 AM.jpeg" alt=""><figcaption><p>Selecting Category for Flows</p></figcaption></figure>

**Editing and Deleting Flows:**

* To **edit** any Flow, click on it and modify the necessary parameters.
* To **delete** a Flow, tick the checkbox next to the flow and click on![](../../.gitbook/assets/Delete.svg). Confirm the deletion on the prompt that appears.

<figure><img src="../../.gitbook/assets/Untitled design (12).png" alt=""><figcaption><p>Deleting a Flow</p></figcaption></figure>

## Flows Logs

Flows logs provide a comprehensive record of automation activities, including:

* **Alarm /Operational Notification Identification**: Identifies which alarm, flight event or operational event initiated the automation routine.
* **Time**: Notes the time at which the Flow was activated.
* **Status**: Shows whether the Flow response was successful or not.

<figure><img src="../../.gitbook/assets/Image 19-02-25 at 1.12 PM.jpeg" alt=""><figcaption><p>Flows Logs </p></figcaption></figure>

**Detailed Log View:**

* Clicking on a log entry opens a detailed view, where you can see:
  * The alarm received and its status.
  * The action taken in response to the alarm and its status.
  * The response mode and the device that responded.
* **Additional Options:**
  * **Rerun Flow**: Allows you to execute the flow again again if required.
  * **Flight Logs**: Access logs from the flight conducted in response to the alarm.
  * On the right, a map is displayed, centered on the alarm's location.

<figure><img src="../../.gitbook/assets/Image 19-02-25 at 1.21 PM.jpeg" alt=""><figcaption><p>Detailed Flows Log</p></figcaption></figure>

{% hint style="info" %}
**Quick Alarm and Flows Logs:**

A **condensed version** of the Alarms and Flows logs can be found in the **Integrations Panel** on the right side of the Dashboard. This panel also displays all Flinks, any alarms triggered within those Flinks. Additionally if a flow is configured with an alarm you can see the response details as well.&#x20;
{% endhint %}

<figure><img src="../../.gitbook/assets/Image 19-02-25 at 1.01 PM.jpeg" alt=""><figcaption><p>Alarms and Flows Logs (Sidebar)</p></figcaption></figure>
