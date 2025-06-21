# Importing a Mission using KML file

When it comes to capturing precision aerial data via aerial surveys, having a good definition of the required area is the starting point for any project. A **KML (Keyhole Markup Language)** file is used to display geographic data (polygon areas and linear paths).&#x20;

This feature reduces the workload of a user when planning complex mission flows with \
FlytBase. Since the format KML is widely known and accepted, it provides users with the ability to create complex missions via the FlytBase dashboard.

{% hint style="warning" %}
The KML file must not contain a flight path, waypoint actions, and curved or circular path.
{% endhint %}

#### Import KML Missions feature is a part of the Mission tab, and can be accessed when the operator clicks on 'add mission'. The user is given the option to create or import either of the two types of missions:

1. **Path mission:** To import a path mission, go to the **missions** tab, click on **'add mission',** and select the **'import mission'** option.\
   The operator can then configure the mission route and waypoint settings. Refer to the path mission tab to set the parameters for the mission.

<figure><img src="../../../.gitbook/assets/kmlgif.gif" alt=""><figcaption><p>Create a Path mission using KML import</p></figcaption></figure>

{% hint style="warning" %}
Please ensure that the KML file does not contain a closed shape when creating a Path Mission.
{% endhint %}

2\. **Grid mission:** To import a grid mission, go to the missions tab, click on '**add mission'**, and select **'import mission'** under the grid mission option. The shape created in the KML file must be a polygon to create a grid mission.

The operator may then configure the grid route and layout settings. Refer to the grid mission tab to set the parameters for the mission.

<figure><img src="../../../.gitbook/assets/gridkmlgif.gif" alt=""><figcaption><p>Create a grid mission using KML import</p></figcaption></figure>

{% hint style="warning" %}
Please ensure that the KML file does not contain more than one shape.
{% endhint %}
