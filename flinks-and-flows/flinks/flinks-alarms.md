# Flinks: Alarms

**Alarm Flink** seamlessly integrates various alarm sources such as sensors, cameras, fences to trigger real-time dashboard notifications or automated workflows via Flows when thresholds are met.&#x20;

### Creating your Alarm Flink

* Navigate to the **Operations Dashboard** and click on the **Navigation Drawer**. From the dropdown menu, select  <img src="../../.gitbook/assets/image (536).png" alt="" data-size="line">  **Flinks.**

![Flink selection on the Operations Dashboard](https://usercontent.clueso.io/b2bb36f5-e45c-4b1c-ba08-2610164f5037/7c298cf0-4fc6-4589-bb56-2af2f3119c31/5c0d2cd4-2b84-4750-8623-e6b8f5e7b3b5/images/010a9aec-4f57-4671-922c-b8c70550b016.png)

* In the **Flinks library**, set up your **Custom Flink** by choosing **Alarms** and clicking on **Next**.

![Adding a custom alarms Flink](<../../.gitbook/assets/Image 19-02-25 at 3.52 PM.jpeg>)

* **Assign a name** to your Flink. Optionally, add a description and an icon. Preview your Flink and click on **Add**.&#x20;
* Your new Flink will now appear in the **My Flinks** section.

![Customizing your Flink](<../../.gitbook/assets/Image 19-02-25 at 4.45 PM.jpeg>)

### Configuring your Alarm Flink

* Go to **My Flinks** and select the Flink you just created. In the **Configuration** section you can assign a specific icon to the alarm.

![Configuring a new Alarm Flink](<../../.gitbook/assets/Image 19-02-25 at 4.54 PM.jpeg>)

* &#x20;After this move to the **Alarm Sources** section. All alarm sources associated with a Flink can be created and managed here. Click on **Add Source** to begin adding a new Alarm Source.
* Here you can enter the **name** and a short **description** of the Alarm Source. After this click on **Generate URL** to proceed.

![Adding a new Alarm Source](<../../.gitbook/assets/Untitled design-6.png>)

*   A follow-up window will display **Source Details**, which include:

    * A **Trigger alarm Webhook URL**. This URL can be used by an Alarm Source to send a notification to FlytBase.&#x20;
    * A sample **JSON Payload** to provide details of the alarm when triggered. User can copy the JSON Payload format, paste it in the relevant environment (used for alarm sensor configuration), and modify the fields of the JSON Payload so that it accepts correct information.&#x20;
    * Users can also test the recently created Alarm Source using the **Test** button. Testing the Alarm Source would only raise an alarm notification on the Integration Panel on the right side of the Dashboard.

    **Note: Pressing the Test button will not trigger any Flows linked to the Alarm Source.**

<figure><img src="../../.gitbook/assets/Image 19-02-25 at 4.55 PM (1).jpeg" alt=""><figcaption><p>Trigger alarm webhook URL</p></figcaption></figure>

* A **Heartbeat URL** to monitor and reflect the status of the alarm source on the FlytBase Dashboard. A **Green** status indicator in front of the alarm indicates an active alarm source.&#x20;

<figure><img src="../../.gitbook/assets/Image 19-02-25 at 4.57 PM (1).jpeg" alt=""><figcaption><p>Heartbeat alarm webhook URL</p></figcaption></figure>

{% hint style="info" %}
These Webhook URLs can be used to integrate third-party sensors such as electronic fences, motion detection and thermal cameras with FlytBase.
{% endhint %}

* To retrieve these **URLs** later, click on the **Source Details** button for the specific alarm source you want to integrate.
* The **Trigger alarm Payload (JSON)** for the Alarm Source contains the following information:

```
//A sample JSON Payload
{
  "timestamp": 1708502346278, //Epoch time elapsed since Jan 1, 1970 in milliseconds
  "severity": 2,              //Integer value in the range 1-3, unknown is 0
  "description": "High temperature!", //User-defined string in double-quotes
  "latitude": 37.7749,        //Source Latitude in decimal format
  "longitude": -122.4194,     //Source Longitude in decimal format
  "altitude_msl": 100,        //Altitude at which the drone hovers over the source
                              //Value should be +ve, and Relative to Take-off (RLT)
  "metadata": {
    "sensor_id": "TempSensor12A", //User-defined additional data for the alarm
    "temperature": 50.2,          //Variable names in "", integers without quotes
    "battery_level": 80           //Strings in ""
  }
}
```

### Alarm Source Logs

Next, click on the **Alarm logs** section, all alarms triggered for the selected Flink are recorded here. You can filter these logs by Alarm Source or by the date they were raised.

<figure><img src="../../.gitbook/assets/Image 19-02-25 at 6.52 PM.jpeg" alt=""><figcaption><p>Alarm Logs</p></figcaption></figure>

### **Modifying and Deleting an Alarm Source**

* To modify an alarm source, tick the checkbox next to the specific alarm to first select it. Click the ![](../../.gitbook/assets/Edit.svg) button located next to the **Add Source** button to update the name and description.

<figure><img src="../../.gitbook/assets/Untitled design-9.png" alt=""><figcaption><p>Editing an alarm source</p></figcaption></figure>

* To remove one or more alarm sources, check the boxes next to the desired alarms. Click the ![](../../.gitbook/assets/Delete.svg)button to delete the selected Alarm source(s).

<figure><img src="../../.gitbook/assets/Untitled design-7.png" alt=""><figcaption><p>Deleting an alarm source </p></figcaption></figure>

***

* After setting up a Flink and alarm sources within it, you will be able to see notifications on the **Integrations Panel** on the right hand side of the dashboard whenever an alarm source is triggered.&#x20;

<figure><img src="../../.gitbook/assets/Image 19-02-25 at 5.54 PM.jpeg" alt=""><figcaption><p>Alarm notifications on the Integrations</p></figcaption></figure>

* Moving forward, you need to create an **automation workflow** to configure response action for the alarm sources from your drone fleet. To learn more about creating such automation workflows, refer to the documentation on[ ](../flows/)[Flows: Alarms](../flows/flows-alarms.md).
