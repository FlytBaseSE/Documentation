---
description: >-
  Map Overlays allows users to import and display 2D maps, enhancing mission
  planning and data accuracy. Operators can easily manage overlays, adjust
  visibility, and ensure precise missions.
---

# Map Overlays

## Overview

Map Overlays allows you to import 2D maps from third-party mapping software and overlaying of them on the FlytBase base map. This feature is useful for users who wish to update outdated and inaccurate mapping data from major map providers. Operators can now accurately plan missions, avoid previously unmarked obstacles, and ensure precise data capture for inspections.&#x20;

## Accessing Map Overlays

To access Map Overlays from the FlytBase Dashboard:

* Click on <img src="../.gitbook/assets/Hamburger Menu.svg" alt="" data-size="line"> to open the **Navigation Drawer**
* Scroll down the list, and click on **Map Overlays**

<figure><img src="../.gitbook/assets/image (601).png" alt=""><figcaption><p>Navigating to Map Overlays</p></figcaption></figure>

## Adding a Map Overlay

To add a new map overlay:

* Click on the ![](<../.gitbook/assets/Create Add (1).png>) to add a new overlay, this would open the import map overlay dialog box.&#x20;

<figure><img src="../.gitbook/assets/image (602).png" alt=""><figcaption><p>Adding a new map overlay</p></figcaption></figure>

* Select the type of Map Overlay. You can choose between 2D imagery, Terrain Data and Point Clouds.

<figure><img src="../.gitbook/assets/Image 4-22-25 at 3.25 PM.jpeg" alt=""><figcaption><p>Assigning site to map overlay</p></figcaption></figure>

* Assign one or more sites where the map overlay would be visible.
* Click on **Next.**
* To upload the overlay, you can either upload a file from your computer, or provide a downloadable link to the file.

<figure><img src="../.gitbook/assets/image (610).png" alt=""><figcaption><p>Importing map overlay using local file</p></figcaption></figure>

<figure><img src="../.gitbook/assets/image (607).png" alt=""><figcaption><p>Importing map overlay using downloadable link</p></figcaption></figure>

* After this, provide a name for the new overlay and click on **Upload**.

## Supported Overlay Formats for Enhanced Map Visualization:

### **2D Map Overlays**

* **TIFF/GeoTIFF (.tif/.tiff)** – Georeferenced orthophotos or scanned maps for flat overlays in mission planning or visual reference layers.
* **PNG (.png) & JPG (.jpg/.jpeg)** – Common raster formats for scanned maps or visual references without geospatial data.

### **Terrain** Map Overlays

* **TIFF/GeoTIFF (.tif/.tiff)** – Ideal for georeferenced imagery used in detailed visualizations.
* **IMG (.img)** – Common in remote sensing applications, offering compatibility with large-scale data.
* **DEM (.dem)** – Digital Elevation Models for accurate terrain profiling and elevation rendering in point cloud visualizations.

### **Point Cloud Map Overlays**

* **LAS (.las)** – Standard for aerial LIDAR data, providing detailed 3D point cloud terrain representation.
* **LAZ (.laz)** – Compressed LAS format with no data loss, ideal for efficient storage and transmission of survey-grade datasets.

## Managing your Map Overlays

The Map Overlays manager allows you to add, delete, edit, and control the opacity of the files present.&#x20;

* Search for a specific overlay by name, or click on the to sort the files by name or date. Additionally you can use the Type and Sites filters to access specific overlays.
* For any particular Overlay, use the **toggle button** to activate/deactivate it.
* The **opacity slider** can be used to set the visibility of the overlay on top of base map tiles and other overlays.

<figure><img src="../.gitbook/assets/image (613).png" alt=""><figcaption><p>Configuring a map overlay</p></figcaption></figure>

* To edit your map overlay in detail, click on the three dots and select **Edit**.

<figure><img src="../.gitbook/assets/image (611).png" alt=""><figcaption><p>Editing a map overlay</p></figcaption></figure>

* Here, you can assign multiple sites to the map overlay and add an optional description.
* Once you’ve assigned the overlay to the required sites and chosen an appropriate opacity, simply click **Save** to update the overlay.

<figure><img src="../.gitbook/assets/image (614).png" alt=""><figcaption><p>Assigning a map overlay to multiple sites</p></figcaption></figure>
