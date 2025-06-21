---
description: Guide on how to plan a grid mission on FlytBase
---

# Grid Mission

A Grid Mission consists of a series of straight-line flight paths that run parallel to each other. These missions are commonly used for imaging and surveying applications. FlytBase enables the creation and modification of grid missions by allowing users to control parameters such as Ground Sampling Distance (GSD), Front Overlap, Side Overlap, and more.

## Plan a Grid Mission

* Go to the **Navigation Drawer** and select the **Missions** tab under the **Planning** section.

<figure><img src="../../../.gitbook/assets/mission tab.png" alt=""><figcaption><p>Missions tab in Navigation Drawer</p></figcaption></figure>

* Click on<img src="../../../.gitbook/assets/image (199).png" alt="" data-size="line">icon to add a mission.

<figure><img src="../../../.gitbook/assets/create new mission.png" alt=""><figcaption><p>Adding a Mission</p></figcaption></figure>

* Under the **Grid** **Mission** section, select **Create Mission**.

<figure><img src="../../../.gitbook/assets/image (27).png" alt=""><figcaption><p>Creating a Grid Mission</p></figcaption></figure>

* Provide a name to the new mission.

<figure><img src="../../../.gitbook/assets/image (523).png" alt=""><figcaption><p>Adding a Mission Name</p></figcaption></figure>

* Assign a **Site** for the particular mission.

{% hint style="info" %}
You can assign multiple **Sites** for a mission.
{% endhint %}

<figure><img src="../../../.gitbook/assets/image (28).png" alt=""><figcaption><p>Assigning a Site for a mission</p></figcaption></figure>

To learn more about **Sites**, refer to the following documentation:

{% content-ref url="../../../getting-started-with-your-flytbase-account/site-management.md" %}
[site-management.md](../../../getting-started-with-your-flytbase-account/site-management.md)
{% endcontent-ref %}

* Add **Tags** to your mission to improve mission management.

<figure><img src="../../../.gitbook/assets/image (525).png" alt=""><figcaption><p>Adding Tags to your mission</p></figcaption></figure>

To learn more about **Mission Management**, refer to the following documentation:

{% content-ref url="../mission-management.md" %}
[mission-management.md](../mission-management.md)
{% endcontent-ref %}

* Simply left-click on the map to create a grid. Adjust the vertices of the polygon according to your preferences. The _**S**_ annotated on the grid represents the Grid Start Point.

<figure><img src="../../../.gitbook/assets/2024-03-05 18-32-21.gif" alt=""><figcaption><p>Creating a Grid</p></figcaption></figure>

* After creating the grid, mission details like the **Total Area** covered, **Estimated Time** to complete, and **Estimated Number of Images** to be taken can be found below **Tags**. This information helps in customizing the mission settings according to user preferences.

<figure><img src="../../../.gitbook/assets/image (30).png" alt=""><figcaption><p>Grid Mission Overview</p></figcaption></figure>

## Configuring Grid Mission Parameters

### 1. Select Payload

Select the drone payload to be used during the mission. You can select either **M30 Payload** or **M30T Payload** based on the available hardware.

<figure><img src="../../../.gitbook/assets/image (526).png" alt=""><figcaption><p>Selecting the drone payload</p></figcaption></figure>

### 2. Select Lens (Imaging Sensor)

Based on the selected payload, you can now select the imaging sensors that would be used while executing the mission.&#x20;

* In the case of **M30 Payload**, you can use the **Wide**-Angle lens.

<figure><img src="../../../.gitbook/assets/image (529).png" alt=""><figcaption><p>Selecting Lens for M30 Payload</p></figcaption></figure>

* In the case of a **M30T Payload**, you have the option to either select the **Wide**-Angle imaging sensor, **IR Mode** imaging sensor, or both. When both sensors are selected, the GSD settings for them are displayed below the Route Altitude tab.

<figure><img src="../../../.gitbook/assets/2024-03-05 18-53-35.gif" alt=""><figcaption><p>Selecting Lens for M30T Payload</p></figcaption></figure>

### 3. Take-off Altitude

The drone achieves a set Take-off Altitude and then proceeds to start the Grid Mission. Following are the different modes that you can select from:

<figure><img src="../../../.gitbook/assets/image (4).png" alt=""><figcaption><p>Take-off Altitude settings</p></figcaption></figure>

* **Default Take-off Altitude**\
  The drone achieves the altitude of Grid Start Point (i.e., Route Altitude), and then proceeds towards it.

<figure><img src="../../../.gitbook/assets/image (5).png" alt=""><figcaption><p>Default Take-off Altitude</p></figcaption></figure>

{% hint style="info" %}
You can set the **Take-off Altitude** for a particular device by navigating to **Devices** -> _Select Device_ -> **Settings** -> **Drone Control**. The take-off altitude you set during mission planning will take precedence over the default values set in **Settings.**
{% endhint %}

* **Safe Take-off Altitude**\
  The drone achieves the 'Safe Take-off Altitude’ and then _diagonally_ proceeds to the Grid Start Point.

<figure><img src="../../../.gitbook/assets/image (6).png" alt=""><figcaption><p>Safe Take-off Altitude</p></figcaption></figure>

<figure><img src="../../../.gitbook/assets/image (10).png" alt=""><figcaption><p>Configuring Safe Take-off Altitude</p></figcaption></figure>

### 4. Altitude Reference, Route Altitude, and GSD

&#x20;There are three types of Altitude References that you can select from:

<figure><img src="../../../.gitbook/assets/image (11).png" alt=""><figcaption><p>Route Altitude modes</p></figcaption></figure>

* **Relative Take-off Point (RLT)** \
  Relative altitude is measured from the take-off point. Additional care should be taken when planning close to ground in uneven terrain. Route/waypoint altitude needs to be adjusted based on terrain height.

<figure><img src="../../../.gitbook/assets/image (12).png" alt=""><figcaption><p>Relative Take-off Point</p></figcaption></figure>

* **Above Sea Level (ASL)**\
  Absolute altitude of the drone as represented in the [EGM](https://en.wikipedia.org/wiki/Earth_Gravitational_Model) model. Use ASL for missions that require global altitude measurements, since the reference is set to the sea level.

<figure><img src="../../../.gitbook/assets/image (13).png" alt=""><figcaption><p>Above Sea Level</p></figcaption></figure>

* **Above Ground Level (AGL)**\
  Altitude set with reference to the ground level. Reliable ground elevation data is essential for using this option safely. This mode is best suited to follow the terrain automatically to maintain a specific elevation relative to the ground at any point in the mission.

<figure><img src="../../../.gitbook/assets/image (14).png" alt=""><figcaption><p>Above Ground Level</p></figcaption></figure>

{% hint style="info" %}
Currently, only RLT Altitude configuration mode is active on the Dashboard.
{% endhint %}

* After selecting the Altitude Reference, you can set the following mission parameters:
  * **Route Altitude:** The altitude at which the drone will execute the Grid mission.
  * **GSD (Ground Sample Distance):**  _GSD refers to the dimensions of a single pixel in an image (cm/px), as measured on the ground_. It is calculated based on the drone's sensor properties and the focal length, as well as the altitude at which the drone is executing the mission.&#x20;

{% hint style="info" %}
The GSD is calculated based on the Route Altitude and vice versa.
{% endhint %}

{% hint style="success" %}
You can also set the Route Altitude by accessing **Settings** -> **Flight Configuration**. The altitude set during mission planning will take precedence over the default value specified for flight altitude in Flight Configuration.
{% endhint %}

{% hint style="info" %}
**Ground Sampling Distance (GSD)** helps in the efficient planning of grid missions. It enables the calculation of the optimal altitude and speed at which the drone should fly to achieve the desired image resolution, ensuring coverage of the target area without unnecessary data overlaps or gaps. For precise measurements, detailed site inspections, and accurate volumetric calculations, a lower GSD is preferable as it captures more detail.
{% endhint %}

### 5. Advanced Mission Settings

You can configure the following mission parameters within **Advanced Settings**: &#x20;

<figure><img src="../../../.gitbook/assets/Image 4-21-25 at 5.04 PM.jpeg" alt=""><figcaption><p>Advanced Mission Settings</p></figcaption></figure>

#### Grid Route Speed

Set the speed at which the drone would fly over the grid flight path.&#x20;

<figure><img src="../../../.gitbook/assets/Grid Route Speed-01.png" alt=""><figcaption><p>Configuring the Grid Route Speed</p></figcaption></figure>

{% hint style="info" %}
The suggested Grid Route Speed is smartly calculated based on the selected Route Altitude and GSD.
{% endhint %}

{% hint style="warning" %}
Changing the recommended Route Speed may impact the amount of images captured during the mission.
{% endhint %}

#### Grid Angle

The grid angle can be adjusted to change the orientation of the grid.&#x20;

<figure><img src="../../../.gitbook/assets/image (17).png" alt=""><figcaption><p>Configuring the Grid Angle</p></figcaption></figure>

#### Route waypoint type

<figure><img src="../../../.gitbook/assets/Image 4-21-25 at 5.08 PM.jpeg" alt=""><figcaption></figcaption></figure>

You can configure the drone’s flight path using the following waypoint options:

* **Linear path**\
  Drone takes a straight path and stops at each waypoint for precise tasks like inspection or image capture.
* **Transits waypoint**\
  Drone flies through each waypoint along a curved path without stopping, ideal for smooth and fast missions
* **Curved route, stops at waypoint**\
  Drone follows a curved path and stops at each waypoint to enable smooth transitions with accurate data capture
* **Curved route, drone continues**\
  Drone moves at a constant speed through curved paths without stopping, perfect for continuous or cinematic flights.
* **Controlled radius**\
  Drone turns at waypoints using a set turning radius for smooth, consistent curves useful in mapping or surveying. The waypoint radius would need to specified here.&#x20;

<figure><img src="../../../.gitbook/assets/Image 4-21-25 at 5.19 PM.jpeg" alt=""><figcaption><p> Controller Radius Settings</p></figcaption></figure>

#### Capture Angle

Following parameters can be set to orient the camera in the desired direction:

* **Gimbal Pitch:** The camera will point up or down depending on the value of this parameter.
* **Drone Yaw:** Set the yaw angle at which the drone would conduct the mission. The yaw angle can be configured relative to the **Flight Path** or **North** depending on the requirements.

{% hint style="info" %}
The drone's yaw is locked at the set angle relative to the reference axis (**Flight Path** or **North**) and will not change as the mission progresses.
{% endhint %}

<figure><img src="../../../.gitbook/assets/Image 4-21-25 at 5.06 PM.jpeg" alt=""><figcaption><p>Setting the Camera Angle</p></figcaption></figure>

#### Image Overlap

Image Overlap parameters affect the percentage of region photographed that would be common between two consecutive images taken along the flight path, or two images taken over adjacent flight paths. Changes in these parameters affect the Route Speed and Grid spacing. Moreover, changes in overlap parameters can affect the time taken to process the images and the quality of output obtained after processing.

<figure><img src="../../../.gitbook/assets/image (19).png" alt=""><figcaption><p>Image Overlap settings</p></figcaption></figure>

* **Front Overlap:** Front Overlap refers to the overlap between two consecutive images taken along the flight path of the drone. It is the percentage of overlap between the front end of one image and the back end of the preceding image. The primary purpose of front overlap is to ensure that there is sufficient coverage and redundancy in the captured images for creating accurate and seamless maps or 3D models. High front overlap is essential for photogrammetry, where multiple viewpoints of the same area are required to stitch the images together accurately.
* **Side Overlap:** Side Overlap refers to the overlap between images captured across adjacent flight paths. It is the percentage of overlap between the side of one image and the side of another image from a parallel flight path. Similar to front overlap, side overlap ensures comprehensive coverage of the area being mapped or modeled. It helps in accurately aligning and stitching together images from different flight lines, crucial for creating uniform, high-quality maps or 3D models without gaps.

<figure><img src="../../../.gitbook/assets/Frontimageoverlap-01.png" alt=""><figcaption><p>Illustration of Front and Side Overlap of images in Grid Mission</p></figcaption></figure>

### 6. Approach Settings

For increased safety and efficiency, users can configure the approach path and speed leading to the starting point of a grid mission. This feature provides greater flexibility in designing and aligning the grid mission to meet specific requirements. The following approach parameters can be controlled:&#x20;

* **Approach Speed**: Set the drone's speed for approaching the mission's starting point.
* **Custom Approach Route**: Use the toggle button to enable a custom approach route. If not enabled, the drone will fly directly from its dock to the grid mission's start point in a straight line.

<figure><img src="../../../.gitbook/assets/capture_20240417124139770.bmp" alt=""><figcaption><p>Custom Approach Route for Grid Mission</p></figcaption></figure>

* **Setting an Approach Route**:
  1. Click on the map to mark the starting point of the approach path.
  2. Drag and drop waypoints (midpoints of straight line segments) between this start point and the grid mission's start point to create the desired approach path.
* **Managing Waypoints**:
  1. Waypoints are listed for easy navigation; use the left and right arrows to view all waypoints.
  2. To remove a waypoint, click on the ![](../../../.gitbook/assets/Delete.svg)icon.

<figure><img src="../../../.gitbook/assets/capture_20240417134404216.bmp" alt=""><figcaption><p>Drone Approach Settings (in Red), and Waypoint toggles (in Green)</p></figcaption></figure>

### 7.  RF Link Loss Condition

This setting defines the drone's behavior in the event of RF link loss. Users can configure it to either continue the mission or initiate a Return-to-Home (RTH) procedure.

<figure><img src="../../../.gitbook/assets/Image 4-21-25 at 6.44 PM.jpeg" alt=""><figcaption><p>RF Link Loss Condition</p></figcaption></figure>

### 8. Positioning Accuracy&#x20;

&#x20; Different positioning accuracy options can be configured here:

* GNSS : Relies solely on satellite positioning to guide the drone. Suitable for operations where centimeter‑level precision is not critical. The accuracy range is as following:
  * Horizontal: ± 1.5 m
  * Vertical: ± 0.5 m
* RTK : Switches to Real‑Time Kinematic corrections for ultra‑precise navigation Recommended for applications requiring ultra‑precise station‑keeping such as mapping using grid missions. The accuracy range is as following:
  * Horizontal: ± 0.1 m
  * Vertical: ± 0.1 m

### 9. Finish Action

Choose the finish action for the drone when it completes the grid mission. Here are the different finish actions that you can configure:

* **Return to Docking Station (RTDS)** - The drone goes back to the docking station.&#x20;
* **Exit Mission and Hover** - The drone hovers at the end point of the grid.&#x20;
* **Go to First Waypoint and Hover** - The drone moves to the start point of the grid and hovers there.

<figure><img src="../../../.gitbook/assets/image (22).png" alt=""><figcaption><p>Finish Action</p></figcaption></figure>

Once all settings have been done, click on **Save** to save the mission. This mission will then appear in the **Missions** tab on the FlytBase dashboard.

<figure><img src="../../../.gitbook/assets/image (25).png" alt=""><figcaption><p>Save Mission</p></figcaption></figure>

<figure><img src="../../../.gitbook/assets/image (29).png" alt=""><figcaption><p>Missions tab</p></figcaption></figure>

To know more on how to **import a mission as a KML file**, refer to the following [documentation](importing-a-mission-using-kml-file.md).
