---
description: >-
  Learn more about the default key bindings, personalize your Keyboard commands
  and verify Controller key bindings prior to using Manual Controls.
---

# Key Bindings

FlytBase enables operators to manually control the drone through the Dashboard during missions or emergencies. In manual mode, the drone can be operated using a keyboard and mouse, or specialized controllers such as a gamepad or joystick. The **Key Bindings** tab on the Dashboard allows you to manage and customize these controls:

* **Customize Key Bindings**: Adjust the key bindings for the keyboard and mouse to suit your preferences.
* **Review Default Bindings**: View the pre-set key bindings for controllers, including the joystick and gamepad.
* **Test Controller**: Use the gamepad simulator to test the functionality of the gamepad.

<figure><img src="../../.gitbook/assets/Key Bindings.gif" alt=""><figcaption><p>Navigating to <strong>Key Binding</strong> Settings</p></figcaption></figure>

{% tabs %}
{% tab title="Keyboard Bindings" %}
### Keyboard Bindings

To access/change keyboard bindings, follow these steps:

* Go to **Key Bindings** -> **Keyboard**
* Click on the required command, and assign a key as per your preference.
* To revert to the original keyboard bindings, click on the **Reset to defaults** button.

<figure><img src="../../.gitbook/assets/Screenshot 2024-10-16 002830.png" alt=""><figcaption><p>Key Bindings: Keyboard tab (Red) and Reset to defaults (Yellow)</p></figcaption></figure>

{% hint style="warning" %}
As of October 15, 2024, the default key bindings for Throttle **Up/Down** have changed from **Space/Shift** to **R/F**, and any custom bindings have been reset. Please verify your key bindings before manually controlling the drone.
{% endhint %}

#### Default Keyboard Commands: Payload Control

<figure><img src="../../.gitbook/assets/image (227).png" alt=""><figcaption><p>Default Payload Control commands using Keyboard and Mouse</p></figcaption></figure>
{% endtab %}

{% tab title="Controller Bindings" %}
### Controller Bindings

* Navigate to **Key Bindings** -> **Controller**

<figure><img src="../../.gitbook/assets/Controller Bindings.gif" alt=""><figcaption><p>Controller Bindings</p></figcaption></figure>

FlytBase currently supports the following Controllers for the Manual flight of the drone:

1. Thrustmaster T.16000M FCS Joystick
2. Xbox 360 Gamepad (Wired)&#x20;

{% hint style="info" %}
Currently, FlytBase does not support custom key bindings for the supported Controllers.
{% endhint %}

### Thrustmaster T.16000M FCS: Key Bindings and Actions

<figure><img src="../../.gitbook/assets/capture_20240419192645624 (1).bmp" alt=""><figcaption><p>Thrustmaster Key Bindings</p></figcaption></figure>

<div><figure><img src="../../.gitbook/assets/image (396).png" alt="" width="498"><figcaption></figcaption></figure> <figure><img src="../../.gitbook/assets/Screenshot 2023-11-24 181632.png" alt="" width="470"><figcaption><p>Thrustmaster Controls</p></figcaption></figure> <figure><img src="../../.gitbook/assets/Thrustmaster 3.png" alt="" width="563"><figcaption></figcaption></figure></div>

### Xbox 360 Gamepad: Key Bindings and Actions

<figure><img src="../../.gitbook/assets/image (398).png" alt=""><figcaption><p>Xbox 360 Commands</p></figcaption></figure>

<figure><img src="../../.gitbook/assets/image (399).png" alt=""><figcaption><p>Xbox 360 Commands</p></figcaption></figure>

The controls of the Xbox 360 Gamepad can be tested using the Gamepad Simulator.

{% hint style="info" %}
Currently, the Simulator is only available for the Xbox 360 Gamepad.
{% endhint %}
{% endtab %}

{% tab title="Gamepad Simulator" %}
### Gamepad Simulator

To test the console keys for the Xbox 360 Gamepad, go to **Key Bindings** -> **Controller** -> **Gamepad**, and click on the **Simulator** button.

<figure><img src="../../.gitbook/assets/capture_20240419192700686.bmp" alt=""><figcaption><p>Key Bindings: Gamepad tab (Red) and link to Gamepad Simulator (yellow)</p></figcaption></figure>

Once done, connect your Xbox 360 joystick and press the keys to test whether the commands are being received appropriately.

{% hint style="warning" %}
Only a **wired** **Xbox 360 Gamepad** is supported on FlytBase.
{% endhint %}

<figure><img src="../../.gitbook/assets/capture_20240419192710006.bmp" alt=""><figcaption><p>Gamepad Simulator</p></figcaption></figure>
{% endtab %}
{% endtabs %}

To learn about how to take **Manual Control** of the drone, refer to the following documentation:

{% content-ref url="../../in-flight-modules/how-to-manage-your-flight-operations/how-to-control-your-drone/manual-drone-controls.md" %}
[manual-drone-controls.md](../../in-flight-modules/how-to-manage-your-flight-operations/how-to-control-your-drone/manual-drone-controls.md)
{% endcontent-ref %}

To learn about **Manual Payload Control**, refer to the following documentation:

{% content-ref url="../../in-flight-modules/how-to-manage-your-flight-operations/payload-controls/manual-payload-controls.md" %}
[manual-payload-controls.md](../../in-flight-modules/how-to-manage-your-flight-operations/payload-controls/manual-payload-controls.md)
{% endcontent-ref %}
