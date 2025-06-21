---
description: >-
  Learn how to interact with and customize maps on the FlytBase Dashboard for
  efficient mission planning and real-time operations, using 2D and 3D map
  views, layers, and overlays.
---

# Maps on FlytBase

## Overview

Maps display geographic areas, including natural features, man-made structures, and other relevant information. FlytBase displays both **2D and 3D maps** on the Operations Dashboard.&#x20;

* **2D** maps provide a **top-down** view for precise mission planning, while **3D** maps help maintain a **safe flight altitude** over natural terrain.&#x20;
* 3D maps provide elevation-aware views, helps in maintaining safe flight altitudes over natural terrain.

This document will guide you on how to use these maps effectively for planning and monitoring drone operations.

## Map Interactions&#x20;

You can interact with the Map on the FlytBase Dashboard using your **keyboard and mouse/trackpad**. Here’s a breakdown of the key actions:

### **1. Viewing Options:**

* **Switch Between 2D and 3D Maps:**
  * On the bottom-right of the Map, Use the **Toggle View** button to switch between 2D and 3D map views.
  * The **Compass** (located above the Toggle View button) shows the current map orientation. The default orientation is **North at the top**.
  * Switching between 2D and 3D views automatically **resets** the map orientation to default.

<figure><img src="../.gitbook/assets/3D_toggle copy.png" alt="" width="540"><figcaption><p>3D Toggle View Button</p></figcaption></figure>

*   **Map Layers:**

    * FlytBase allows you to customize the visible layers on the map to suit to your needs.



    *   **Base Layers:**&#x20;

        * **Satellite** (default): Provides a realistic view of the terrain.
        * **Transit**: Displays simplified map visuals with emphasis on roads and boundaries.


    * **Additional Layers:** Enable or Disable additional layers for more detailed information.
      * **Map Labels**: Adds labels (e.g. names of streets) to the Satellite layer.
      * **Annotations**: Shows user-defined markers on the map.
      * **Geofences**: Displays the geographic boundaries that user has created for operations.
      * **No-Fly Zones (NFZs)**: Highlights the created restricted areas for drone flights.
      * **Map Overlays**: Adds high-resolution, site-specific images directly on the 2D Base Map.

<figure><img src="../.gitbook/assets/map layers.png" alt="" width="563"><figcaption><p>Map Layers</p></figcaption></figure>

### **2. Navigating the Map:**

* **Pan the Map:**
  * Hold left-click and drag the mouse to move the map in any direction.
* **Rotate the Map:**
  * Hold the center mouse wheel (if clickable) or press Ctrl + left-click, and drag the mouse to rotate the map in 2D or 3D view.
  * The compass shows rotation and is located above the Toggle View button. Switch to 2D view to reset to default orientation (North on top).

### **3. Zooming In and Out:**

* Use the on-screen + and - buttons.
* Scroll with your mouse wheel.
* Hold right-click and move your mouse up or down.
* Swipe up or down with two fingers on your trackpad.

<figure><img src="../.gitbook/assets/ZoomInZoomOut copy.png" alt="" width="504"><figcaption><p>Zoom-In (+) and Zoom-Out (-)</p></figcaption></figure>

### **4. Centering the Map:**

Click to center the map on:

* Docking Station
* Drone
* Your location

<figure><img src="../.gitbook/assets/Screenshot 2024-12-26 at 10.56.25 AM.png" alt="" width="464"><figcaption><p>Centering the map</p></figcaption></figure>

## Map Tiles and How to Update Them

* FlytBase uses map tiles and services provided by Cesium. Depending on the area, the map tiles may not be updates over a significant amount of time.&#x20;
* Thus, the latest changes in the local terrain or changes at a fast-evolving site may not be reflected on the map. To mitigate this, Flytbase supports [**Map Overlays**](map-overlays.md).&#x20;
