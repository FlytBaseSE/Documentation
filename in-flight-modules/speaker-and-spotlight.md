---
description: >-
  Learn how to configure and use the speaker and spotlight payload using
  FlytBase.
---

# Speaker and Spotlight

With FlytBase, you can easily manage speaker and spotlight payloads on your drone. Here's what you can do:

* **Save and Broadcast Announcements:** Store messages, or draft a quick message, and use the text-to-speech feature to make announcements.
* **Adjust Spotlight Settings:** Change the brightness and switch between spotlight or strobe modes.
* **Activate Siren:** Set off a siren sound and strobe light to indicate a critical situation or to deter intruders.

Such systems enhance your drone's capabilities for perimeter security or search and rescue applications.

{% hint style="info" %}
Currently, the speaker and spotlight payloads supported include:

* For **DJI Dock 1/M30 Series** drones (M30, M30T): **CZI LP12**
* For **DJI Dock 2/M3D Series** drones (M3D, M3TD):&#x20;
  * **JZ M3D Quick Search Kit**
  * **Cytop MLV3D**
  * **CZI MP20**

Reach out to **support@flytbase.com** to know more.
{% endhint %}

## Speaker

### Adding Announcements

To add announcements to a payload, follow these steps:

* **Attaching the Payload**: Attach the payload to the drone, and power on the drone.
* **Navigating to the Payload Tab**: On the FlytBase Dashboard, go to the **Device Management** section, and select the **Payload** tab.

<figure><img src="../.gitbook/assets/Screenshot 2025-01-23 at 2.53.47 PM.png" alt=""><figcaption><p>Payload Tab for the selected device</p></figcaption></figure>

The Payload tab allows you to perform the following operations:

* **Add Audio for playback:** You can add audio files that can be played by any drone using its payload.

<mark style="color:yellow;">\[ modify this section so that an image for this feature is added ] \[You can do two things in payload section - add audio files, or add text announcements ]</mark>

* **Creating an Announcement**: Click on the **Add** button. This action will bring up a dialog box where you can configure your announcement. In the dialog box, enter a name for your announcement and type your announcement text.&#x20;

{% hint style="warning" %}
Announcement text cannot exceed 200 characters.
{% endhint %}

<figure><img src="../.gitbook/assets/Image 23-01-25 at 2.59 PM.jpeg" alt=""><figcaption><p>Adding a new announcement</p></figcaption></figure>

* **Saving the Announcement**: After entering your information, click **Save** to finalize the announcement.

{% hint style="info" %}
You can create up to twenty announcements for each payload.
{% endhint %}

<figure><img src="../.gitbook/assets/Image (1).png" alt=""><figcaption><p>Saved announcements</p></figcaption></figure>

### Operating the Speaker

To use the Payload, navigate to the **Fleet view** and select the **Payload** ![](<../.gitbook/assets/Payload icon.svg>)icon adjacent to the drone video feed widget.

The payload widget would expand, allowing access to speaker and spotlight tabs.

<figure><img src="../.gitbook/assets/GTL.png" alt=""><figcaption><p>Expanded Payload widget</p></figcaption></figure>

#### Play a saved Announcement

* In the expanded Payload widget, click on the **Speaker** tab.
* Choose the desired announcement from the list of saved announcements and click **Play**.
* To keep repeating the selected message, click on the ![](../.gitbook/assets/Icon.png) icon. The message will be repeated as long as the ![](../.gitbook/assets/Icon.png) icon is not pressed again or message playback is stopped from the Play/Stop button.

<figure><img src="../.gitbook/assets/Select announcement highlighted.png" alt=""><figcaption><p>Select Announcement </p></figcaption></figure>

#### Quick Announcement

For making an urgent custom announcement:

* Type your message (up to 200 characters) in the **Quick Announcement** box.
* Click **Play** to broadcast your message immediately.

<figure><img src="../.gitbook/assets/quick announcement highlighted.png" alt=""><figcaption><p>Quick Announcement</p></figcaption></figure>

{% hint style="warning" %}
Quick announcements are not stored in the list of Saved Announcements.
{% endhint %}

#### Speaker Volume Settings

Adjusting the speaker volume:

* Use the volume bar to increase or decrease the volume according to your preference.
* The volume can be adjusted within a range from 0 to 40.

## Spotlight Settings

If the payload includes a controllable spotlight (such as in LP12), it can be operated through the Payload widget.

**Activating the Spotlight**

To control the spotlight:

* Click on the **Spotlight** ![](<../.gitbook/assets/noun-flashlight-218765 5.svg>) in the **Payload** widget.&#x20;
* Use the **toggle button** to turn the spotlight on or off.

**Adjusting Brightness**

Adjust the brightness of the spotlight:

* Move the **brightness slider** to the right to increase brightness or to the left to decrease it.

**Spotlight Modes**

The spotlight offers two modes:

* **Static Mode**: The spotlight remains continuously on at a consistent brightness.
* **Strobe Mode**: The spotlight alternates between on and off, creating a pulsating effect.

<figure><img src="../.gitbook/assets/Frame 427321742 (2).png" alt="" width="290"><figcaption><p>Spotlight Controls</p></figcaption></figure>

## Siren

If the payload is equipped with a Siren feature, you can activate it through the **Payload** widget on the FlytBase Dashboard.&#x20;

**How to Activate the Siren**

* Navigate to the **Payload** widget.
* Locate the **Siren** button at the bottom of the widget; this button is common for both the speaker and the spotlight.
* Click the **Siren** button to activate the siren, which switches on the spotlight in strobe mode and plays the default siren sound.

<figure><img src="../.gitbook/assets/image (563).png" alt="" width="248"><figcaption><p>Siren button</p></figcaption></figure>
