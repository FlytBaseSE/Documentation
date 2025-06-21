# Device Maintenance

## Maintenance

This section allows operators to check the Docking Station's real-time health status and enables them to perform maintenance controls and Docking Station commands.

### Docking Station

#### **Docking station status**&#x20;

The docking station health card indicates the current status of the docking station. The docking station has the following states:

* **Remote debugging:** When the docking station is undergoing maintenance from the control station i.e., in the FlytBase application, the status will be displayed as remote debugging.
* **Onsite debugging:** When any binding/debugging activity is being performed on-site directly from the docking station, the status will be displayed as onsite debugging.
* **Idle:** When the docking station is not in use, the status will be displayed as Idle.
* **Docking Station Storage:** The docking station storage provides information about the available data and total storage capacity of the docking station.

<figure><img src="https://lh4.googleusercontent.com/KYaHKw9xBv-KkZ1_Ri6D--n58S1Cc2VBMINrF7tjsEHkY-78Km7G6SQTjTWfGqJAgTRzATRFQSHD4cWI7AfwAicULIHJg-utSZEx7CjlRxT-B_xDZvVT6YEjOyXqeOmWmWu8qU7XCQU9HergzRE8qQ" alt=""><figcaption><p> Maintenance window</p></figcaption></figure>

#### **Video feed**

The docking station health includes the video feed from the Docking station camera. You can toggle the available video feed on or off as needed for viewing.

#### **Docking station position**

The docking station's position in the health status indicates the GPS health status of the docking station.

* **GPS Fix**: The GPS fix indicates the current GPS health of the GPS system in the docking station.&#x20;
  * **“Fixed”** status means the GPS position is locked and is ready for missions.  &#x20;
  * **"Open"** status means the GPS position is not locked and not ready for missions. The drone cannot take off with this status.
* **GPS Satellites**: The GPS satellite count represents the number of satellites that the docking station can lock onto for accurate positioning. If the satellite count is low, the docking station will not allow any flights.&#x20;
* **RTK Satellites:** The RTK satellite count refers to the number of satellites available for RTK (Real-Time Kinematics) to achieve precise landing on the docking station after a mission. If the RTK satellite count falls below the required threshold, the docking station will not allow precision landing on the docking station. Instead, the drone will move to the alternate landing site for landing that is set by the user.&#x20;

<figure><img src="https://lh4.googleusercontent.com/8wPhWsvfDZy5RO2X1nt5lv-PoAK6VKcUGY4WUFH0BC6ZM7D7KVHDkWK9nPFCCGfFXxRzzogbswIYjNWrrQQviN0B8369-KzKSqIvcvNSmcu8J8jLDeW9uiDweg_UM9OGHDnvqWWU245IXAMuWtcD4w" alt=""><figcaption><p>Dock Position</p></figcaption></figure>

#### Environment:

The environment card allows you to monitor the H.V.A.C (Internal) values of the docking station as well as Weather (External) conditions.&#x20;

{% hint style="info" %}
H.V.A.C stands for Heating, Ventilation, and Air Conditioning unit.
{% endhint %}

The following parameters can be monitored:

* **H.V.A.C (Internal)**:&#x20;
  * **Temperature**: The temperature of the docking station can be monitored with this information card.  Temperature is measured in degrees Celsius by default.&#x20;
  * **Humidity:** The humidity of the docking station can be monitored with this information card. Humidity is measured in kilo Pascals by default.&#x20;
  * &#x20;**H.V.A.C state:** The status and functionalities of the H.V.A.C units are explained below:
    * Idle: The H.V.A.C. unit is in idle condition.
    * Heating: The H.V.A.C. unit has initiated heaters to increase the temperature and increase back to the ideal temperature for the docking station’s use.
    * Cooling: The H.V.A.C. unit has initiated coolers to reduce the temperature and reduce it back to the ideal temperature for the docking station’s use.
    * Dehumidifyin&#x67;**:** The H.V.A.C. unit has initiated dehumidifiers to reduce the humidity of the docking station. This enables the docking station to maintain standard conditions for efficient usage.&#x20;
* **Weather (External)**: The weather card provides information on the external weather conditions at the docking station’s location, using the integrated weather station in the docking station.
  * Temperature: External temperature conditions of the docking station can be monitored using the integrated weather station attached to the docking station. Temperature is measured in degrees Celsius by default.&#x20;
  * Wind: Wind speed at the location of the docking station can be monitored using the integrated weather station attached to the docking station. Wind speed is measured in meters per second by default.&#x20;
  * Rain: Rain at the location of the docking station can be monitored using the integrated weather station attached to the docking station. Rain is measured in millimeters by default.

#### Network

The network card in the Maintenance tab allows you to monitor the network parameters of the docking station. And would display the following:

* Type: The type of network used is displayed in the Network card.
* Ethernet: When ethernet is used as a network source for the docking station, ethernet is shown in the network card. &#x20;
* Quality: The quality of the internet connection to the docking station is displayed on the network card. Quality can be rated Poor, Average, and Good as per the data transfer speed.&#x20;
* Rate: The rate of data transfer to and from the docking station through the network utilized is displayed in the Network card.&#x20;

<figure><img src="https://lh6.googleusercontent.com/-i5euN-JdfgG_n3TBIMtfB2PyFcQQa2qPiFxhaoUccoGDzyM6YwopzG8WdqvplnE-0NpZQ1ET2iwJtHcYVCrqJtOeZL3xscKNv9aCwjkIY_hXYotq5iDkRVLKCY7mqsOuQtEFJMWAuz5W4pwzKqFtg" alt=""><figcaption><p>Network status of the dock</p></figcaption></figure>

#### **Power Source**

The power source card provides data related to the power being received by the docking station.

* Voltage: The voltage of the power source is displayed on the power source card. The input voltage that is recommended for the docking station is 100-240 V AC.&#x20;
* Current: The current usage of the power source is displayed on the power source card. The input current that is recommended for the docking station is 6.25 to 15 A.

<figure><img src="https://lh3.googleusercontent.com/vyNTbe3F91qcewknzSMfs-W81be08saHP__GocKAw_9VRFcUit39CiOruHXZBm89wxSojOntVvYQSsYFkA27tTWYs6vPMeEW-Qjlv4-arPpVcVE3mEE0IPov7-Pm6JKgfvCGFTku5EKo8aq-o1fMmQ" alt=""><figcaption><p>Power Source</p></figcaption></figure>

#### Backup Battery

The backup battery panel displays information about the backup battery.

* Switch: If the backup battery is powered on, the switch is displayed as closed; otherwise, it is displayed as open.
* Backup Voltage: The voltage supply of the backup battery is displayed in the corresponding column.
* Temperature: The temperature of the backup battery is displayed under the temperature column of the backup battery panel.

<figure><img src="https://lh5.googleusercontent.com/exM-y8ArxU-0BSENmLm2Pbb4uZsgQHkZd9l1imfeHCoJUkvbNPflGmLz32pZfDu_W8NOl9TNGzqmsh_c_OWPJMnSPd8pQyUFGiQStRL7_TJMLY5QYZ5AE-rOOFnfLVq7BvJqQCSeBW3oJRJv4jSgUQ" alt=""><figcaption><p>Backup Battery</p></figcaption></figure>

### Drone

#### Drone Health

The maintenance tab in the devices feature allows you to monitor the health parameters of the drone along with the docking station.

* Drone status: The current status of the drone can be monitored in the drone status section. The status displayed here represents the real-time data of the drone.&#x20;
  * Standby: This status indicates that the drone is ready for flight.
  * Upgrading firmware: This status Indicates that the firmware in the drone or battery is being updated.
  * Automatic Take-off: This status indicates that the automatic take-off sequence has been initiated.
  * Wayline flight: This status indicates that the drone is performing an auto mission.
  * Automatic return: This status indicates that the Return To Home (RTH) procedure has been initiated and the drone is returning to the docking station.
  * Automatic landing: This status indicates that the drone is landing on the docking station after completing a mission or during RTH.
* Control Source: The control source card refers to the source of control of the drone, two options it can be controlled:
  * RC: The drone can be controlled using the RC provided with the drone.
  * Docking Station: The drone can be controlled by the docking station, either by planning autonomous missions or by using Keyboard/external joysticks to control the drone manually.

<figure><img src="https://lh3.googleusercontent.com/aS39SU2HrUhSZ9cpOhQNVtc5jLLHdHXRRRX78QaPPCpfSPDB8-UL2K5KUetQyrGE7XiUuMBsN8mLUK8yLJEQ1L3FDZsLTkbfkjBzSrHN1WEfPZDapzzskSl8veNNVkvyB1ey8DM-OQ9f9OF6caIi7A" alt=""><figcaption><p>Drone Health Status</p></figcaption></figure>

#### Drone Storage

Similar to the docking station, the total storage allocation and available storage space of the drone are displayed in the drone storage card.

#### Drone Video Feed

The drone video feed panel allows you to view the live video feed from the drone during flight as well as when it is sitting idle in the docking station.

#### Drone Position:&#x20;

The position of the drone in the Health status indicates the GPS health status.&#x20;

* **GPS Fix**: The GPS fix indicates the current GPS health of the drone.&#x20;
  * &#x20; “Fixed” status means the GPS position is locked and is ready for missions.&#x20;
  * &#x20; "Open" status means the GPS position is not locked for missions. The drone cannot take-off with this status.
* **GPS Satellites**: The GPS Satellites count represents the number of satellites that the drone can lock onto for accurate positioning. If the satellite count is low, the docking station will not allow any flights.
* **RTK Satellites**: The RTK satellite count refers to the number of satellites available for RTK (Real-Time Kinematics) to achieve a precise landing on the docking station after a mission. If the RTK satellite count falls below the required threshold, the docking station will not allow precision landing.

Battery

The status of the battery can be monitored in the drone's health status.&#x20;

<figure><img src="https://lh4.googleusercontent.com/Yzj1yVGPH0LyB1-1N9PGkWLN2HjhTgbCBgy3feUpXil6ErucAR9XykYLgJC19-GQHgCzAbqkxhVAGpjaoqkYQ9XGQ6yCdPOeTLfuR9yhQi5Y9WtXgJBwxTIVFfUQ-I3Xi8FtEOmTY-0WIAKtGIjLBA" alt=""><figcaption><p>Aircraft Battery State</p></figcaption></figure>

* Remaining Battery: The remaining battery percentage is displayed, allowing the drone to automatically trigger relevant failsafe actions based on the percentage of battery the failsafe is set to.&#x20;
* Temperature: The current temperature of the battery is indicated while the drone is powered on, in flight, or on the ground.
*   Voltage: The current voltage of the battery is displayed when it is powered ON.


* Battery temperature regulator: The battery temperature regulator ensures that the battery temperature is regulated.&#x20;
  * Maintenance status: The maintenance status indicates whether the batteries require maintenance or not. The drone will carry out the maintenance as it has a battery temperature regulator.&#x20;
    * Need Maintenance: This is displayed when the battery requires maintenance.&#x20;
    * No Need: This is displayed when the battery doesn’t require maintenance.
    * Under Maintenance: This is displayed when the battery is under maintenance.&#x20;
* Battery Status: The battery status indicates the insulation or heating status while using the Battery temperature regulator. It can indicate whether the battery is insulating, heating, or neither.

<figure><img src="https://lh5.googleusercontent.com/ncLqp3mEBLUg02AHOmGDgNOJJhGKe2DlvfvyZT4l6HRXewn7Fv6c_Tvo0wLFGQ67rBsLYQmfN18chlAIPgH_a325paPXjibmPlZgJAFaPn06XRCRP_cOl2P5rArW9AWpKxpStC_moJrAk2C5Xm6Q1g" alt=""><figcaption><p>Battery Temp. Regulator State</p></figcaption></figure>

### Device Controls

#### Docking Station:&#x20;

The following actions can be performed from the docking station section.

* **Heater:** The heater in the docking station's H.V.A.C system can be controlled by using the “ON/OFF” toggle button.
* **Cooler:** The cooler in the docking station's H.V.A.C. system can be controlled by using the “ON/OFF” toggle button.
* **Dehumidifier:** The dehumidifier in the docking station's H.V.A.C system can be controlled by using the “ON/OFF” toggle button.
* **Sound & Light Alarm:** The sound and light alarm in the docking station can be controlled by using the “ON/OFF” toggle button.
* **Camera Light:** The camera light in the docking station can be controlled by using the “ON/OFF” toggle button.
* **Dock Silent Mode:** Turning this mode ON reduces the operational noise of the dock, providing a quieter environment during drone operations.&#x20;

{% hint style="warning" %}
Enabling the Silent Mode may slightly affect the cooling performance of the Dock's air conditioning system.
{% endhint %}

* **Drone Stealth Mode:** Turning this mode ON reduces the visibility of the drone by dimming its lights, ensuring discreet drone operations.
* **Docking and Drone Storage:** The Dock and Drone storage can be formatted using the “FORMAT” button in the device control section.

<figure><img src="../../../.gitbook/assets/image (594).png" alt="" width="563"><figcaption><p>Device Controls</p></figcaption></figure>

### Device Maintenance

The operator must enable Maintenance to perform the actions mentioned below.

&#x20;When enabled, the Docking Station Status will switch to 'Remote Debugging'.

The following actions can be performed for Device Maintenance:

* Docking Station Power: The docking station can be restarted using the “RESTART” button available in the device controls section.&#x20;
* Docking Station Enclosure: Enclosure of the docking station can be opened or closed using the “OPEN/CLOSE” toggle button.&#x20;
* Docking Station Charging Rods: Charging rods of the docking station can be opened or closed using the “OPEN/CLOSE” toggle button.&#x20;
* Drone Power: Drone power can be turned on or off using the “ON/OFF” toggle buttons in the device controls section.&#x20;
* Drone Charging: Drone charging can be turned on or off using the “ON/OFF” toggle buttons in the device controls section.&#x20;
*   Drone Battery Temp. Regulator: The battery temperature controls of the drone can be turned on or off using the “ON/OFF” toggle buttons in the device controls section. \


    <figure><img src="../../../.gitbook/assets/image (279).png" alt=""><figcaption><p>Device Maintenance</p></figcaption></figure>

{% hint style="success" %}
Please Disable the Maintenance mode before performing flights.
{% endhint %}



Next up, learn how to effectively use the [Health Management System](diagnostics.md) in the FlytBase platform.
