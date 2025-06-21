---
description: >-
  Fleet 2.0 supports 3D Map Visualization which allows you to monitor your
  operations spread out in different sites along with live tracking and
  interative map features with the ability of auto tracking
---

# Interactive 3D Map Visualization

## Overview

The Interactive 3D Maps provide an advanced interface for real-time geospatial monitoring and control of drone operations. This includes support for live asset tracking, flight path visualization, and interactive map features.

## Map Behavior and Interaction

#### Default Centering

* Upon initialization, the map automatically centers on the user’s current location to provide immediate operational context.

<figure><img src="../../../.gitbook/assets/Image 29-05-25 at 3.46 PM.jpeg" alt=""><figcaption><p>Default View </p></figcaption></figure>

#### Dynamic Re-centering

* When a drone is made visible in the interface, the map automatically recenters to include the drone's current location.

<figure><img src="../../../.gitbook/assets/image (624).png" alt=""><figcaption><p>Map centered to current drone location</p></figcaption></figure>

* If multiple drones are selected as visible, the map dynamically zooms out to ensure all selected drones are within view.

<figure><img src="../../../.gitbook/assets/Image 29-05-25 at 3.49 PM.jpeg" alt=""><figcaption><p>Map zooms out to focus on two different sites in view</p></figcaption></figure>

* In cases where drones are geographically dispersed, the zoom level may adjust to a global view to accommodate all visible assets.

#### Spotlight Tracking Mode

* Pinning a drone activates Spotlight Mode, enabling map tracking of the pinned drone’s movement.

<figure><img src="https://lh7-rt.googleusercontent.com/docsz/AD_4nXe-WprLXQUiElCl1hrjLVwZYDZrCCsRmjmZWNuc8-XN6hgaLFfcuXcDdEEAg8VXVYAoP0vU27gQtJzE_Fhvlx2FQyn8revBIcYmI0h1sOgCl4zAGRgT-wWFPIr7MyWxX4y6OD5d?key=h8fUn6alQ99iBpzkBxQitA" alt=""><figcaption></figcaption></figure>

* In Spotlight Mode, the map automatically follows the pinned drone.
* Tracking can be disabled by the user to allow manual interaction with the map.

<figure><img src="../../../.gitbook/assets/Image 29-05-25 at 3.56 PM.jpeg" alt=""><figcaption><p>Turning off auto tracking</p></figcaption></figure>

## Features

#### Real-time Drone Positions

* All active fleet assets are displayed on the map with real-time position updates.

#### Flight Path Visualization

* The current location of each drone is displayed.
* A visual flight path is rendered as a blue trajectory line representing the drone's recent movement.

#### Site Locations

* All drone dock locations and operational sites are clearly marked on the map for reference and planning.

#### Airspace Threat Overlay

* Airspace threats are overlaid on the map to indicate potential hazards or conflict zones.

#### Zoom and Navigation

* The map supports full 3D interaction capabilities, including pan, zoom, and rotation.
* Users can freely navigate the map to inspect specific areas or monitor fleet operations in detail.



<div align="center"><figure><img src="https://lh7-rt.googleusercontent.com/docsz/AD_4nXeLJrOmTG89mMEYG7VSmPyFZnsaMC3agbW1QXitxwzRMFckrXxELtYUoIngkdvdp4sVIL8NxFPvs98HxnvMQ_0OL-0YeBb8WwgGHkrlqUrx44fw4fpGjJdsNuci9Nc_kT3EJJ7CpQ?key=ltwtiAhGhp6bUzvxpSYaXw" alt=""><figcaption><p>Interactive 3D map displaying airspace threats with altitude information, drone positions, flight paths, and docking stations with comprehensive geospatial awareness.</p></figcaption></figure></div>

## Additional Notes

* Only one drone can be pinned at a time.
* Drone tracking can be toggled on or off to switch between automatic following and manual map control.
