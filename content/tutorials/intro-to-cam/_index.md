---
title: Intro to CAM with Fusion 360
description: Getting started with Fusion 360 CAM
src: https://docs.google.com/document/d/1EK63A9zoJkVzYDzSKFMsQuw_GsHjY60yi7C2bry6HIY
weight: 10
---

This is a brief introduction/refresher for creating GCODE via Fusion 360 CAM. This guide assumes CAM is targeted at the Velox using Mach3 as the GCODE sender.

1. Download a STEP file of the part from Onshape {{< expand "Show Me..." >}}
{{< columns >}}
<img src="onshape-export.png">
<---> <!-- separator between columns -->
<img src="onshape-export-type.png">
{{< /columns >}}
{{< /expand >}}

2. Open the file in Fusion 360 {{< expand "Show Me..." >}}
- [How to import or open a file in Autodesk Fusion 360](https://knowledge.autodesk.com/support/fusion-360/learn-explore/caas/sfdcarticles/sfdcarticles/How-to-import-or-open-a-file-in-Autodesk-Fusion-360.html)
{{< /expand >}}
3. Be sure the part is laying down with the correct **face up**. We have had the most success when the **part top face matches Fusion's Top orientation**. For some parts it will not matter which face is up. {{< expand "Show Me..." >}}
![](fusion-orientation.png)
1. Locate the part in the browser under the Bodies section. Select the part by clicking on it once ![](fusion-bodies.png)
2. Open the Move/Copy dialog by pressing the 'm' key on your keyboard ![](fusion-move-copy.png)
3. Be sure that **Bodies...** is selected in the **Move Object** dropdown 
4. Use the handles to move/roate the part ![](fusion-rotate-body.png)
5. Click OK when complete. Part should look like this. Notice the orientation of the part and the view cube. ![](fusion-orientation-desired.png)
{{< /expand >}}

4. Change to the Manufacturing workspace {{< expand "Show Me..." >}}![](fusion-manufacture.png){{< /expand >}}

5. Create a Setup which defines what your stock material shape and size are. {{< expand "Show Me..." >}}
Click the folder icon to create a setup.
![](fusion-create-setup.png){{< /expand >}}
6. In Tab 1: Set the **zero axis to the bottom left corner** of the stock so the red and green arrows **point into the stock**. It is critically important that the point selected is used as the zero point when setting up the machine. Be sure to select the the point at the **top of the stock**. {{<expand "Show Me..." >}}
{{< columns >}}
![](fusion-setup-oigin-axes.png?height=180px)
<--->
![](fusion-setup-tab1-origin.png?height=280px)
{{< /columns >}}
   {{< /expand >}}
7.  Measure the **actual z height** of your stock using calipers. (Incorrect z will cut into the table or not cut all the way through.) {{<expand "Show Me..." >}}![](measure-stock-thickness.jpg?height=180px){{< /expand >}}
8. Tab 2: Change **Mode** to **Fixed Size Box**, any mode can be used to best represent your actual stock material. (This guide assumes Fixed Size Box)
8. Tab 2: Make sure the top of the part is aligned with the **top of the stock** in the setup. (This is especially important if your model is a different thickness than your stock.)  {{<expand "Show Me..." >}}![](fusion-setup-tab2-stock-size.png?height=280px)
1. Be sure the **Model Position** dropdown has **Offset from Top** selected
2. be sure the offset is **0 in**
{{< /expand >}}

9. Tab 3: If machining tubes set the WCS (work coordinate system) to 6 to indicate the vises that are setup on our Velox. (WCS6 is pre-configured in the Mach3 software on the PC connected to the Velox.) {{<expand "Show Me..." >}}![](fusion-setup-tab3.png?height=180px){{< /expand >}}
10. Close the setup window by clicking **OK**
    
11. Now that the setup is done, you can create operations to make your part.
    1. If you haven't already import the CAM templates. <a href="{{< relref "import-cam-templates" >}}" target="__blank">Here's How</a>
    2. Next, See <a href="{{< relref "using-cam-templates" >}}" target="__blank">How to Use the CAM templates</a>




