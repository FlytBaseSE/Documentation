# Flows : Alarms

## Setting up a new Flow with Alarms

To create a new Flow, please follow the following steps:

* Go to the **Flows** section on your dashboard, click on the **Create** button.

<figure><img src="../../.gitbook/assets/Untitled design (11) (1).png" alt=""><figcaption><p>Navigating to Flows</p></figcaption></figure>

* A dialog box will appear, prompting you to select a category. Choose **Alarms** from the menu.

<figure><img src="../../.gitbook/assets/Image 18-02-25 at 8.59 PM.jpeg" alt=""><figcaption><p>Creating a Alarms Flow</p></figcaption></figure>

* Enter a **Name** for your new Flow.
* Under the **Trigger** drop-down, select the **Alarm sources** to associate with this Flow.

{% hint style="info" %}
You can link multiple Alarm sources to a single Flow if they require a common response action while each Alarm source can only be linked to one Flow to ensure a consistent response.
{% endhint %}

<figure><img src="../../.gitbook/assets/Image 18-02-25 at 9.19 PM (1).jpeg" alt=""><figcaption><p>Name and Alarm Source(s) selection </p></figcaption></figure>

*   Choose the **Action** the drone will perform in response to the alarm:

    * **Go to alarm location**: Directs the drone to the alarm’s location.
    * **Perform mission**: Carries out a specific pre-existing mission at the alarm’s location.


*   Select the **Response Mode**:

    * **Manual**: The Dashboard prompts you to select an action in response to the alarm when it is triggered.
    * **Automated**: The drone automatically executes the selected action without operator intervention when an alarm is triggered.


* **Associate with a Site**: Select a site to filter out the devices that will respond when the alarm is triggered.
* **Select a Device**: This device will respond to the alarms and carry out the necessary action.&#x20;
* **Device Selection and Response Mode:**&#x20;
  * **Manual Mode:** Select the device during setup or when the alarm is triggered.
  * **Automated:** Requires a mandatory selection of device during setup.

{% hint style="warning" %}
Only one device can be associated with a Flow.
{% endhint %}

* **Action Go To Location/ Performing Mission:** Depending on the chosen Action, either select a pre-existing mission associated with the site or set parameters for the **Go-to Location** maneuver.
* An **Overview** of the flow can be viewed on the right side of the screen.
* Once all the parameters are set, click on the **Create** button and your alarm flow will show up in **My Flows**.

<figure><img src="../../.gitbook/assets/Image 19-02-25 at 12.35 PM.jpeg" alt=""><figcaption><p>Selecting a Device, and setting Go-to Location parameters. Overview in right corner.</p></figcaption></figure>
