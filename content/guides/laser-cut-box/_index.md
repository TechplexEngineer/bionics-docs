---
title: Laser Cut a Box
description: How to use the laser cutter to make a box using Laserjoint and AutoLayout
weight: 50
---

We have been working to organize our toolboxes, and in the process making custom sized organizers for the drawers. Here is a quick guide on how we turn the 3D models into lasercuttable files.

## Design the Box

1. Start with a base sketch. ![](1_base_sketch.png)
2. Extrude the base and walls to individual parts. Here I used an extrude for the base, all the vertical walls and then the horizontal walls. ![](2_design_box.png)

## LaserJoint
3. Use the laser joint tool [(get it here if you don't have it)](/robots/cad/). Select all of your parts, be sure they overlap. ![](3_laser_joint_settings.png)
4. Should now have a box that we can laser cut! ![](4_laser_joint_applied.png)

## AutoLayout
5. We can use the AutoLayout featurescript [(get it here if you don't have it)](/robots/cad/) to make a flattened view of our parts. The laser is 24" bu 18". ![](5_auto_layout_settings.png)
6. Now we have our parts nicely laid out, we now need to export this for cutting. ![](6_auto_layout_result.png)

## Export
I've found the best way is to create an assembly and add all the parts to the assembly at the same time to preserve the layout. If you change your design, you will need to re-insert your parts. 


7. Create a new Assembly ![](7_create_assembly.png)
8. Click the insert button ![](8_insert.png)
9. Select the entire part studio to insert ![](9_insert_all_parts.png)
10. Should now have an assembly of all the flat parts to cut. ![](10_assembly_has_all_parts.png)

11. Create a drawing of the assembly ![](11_create_drawing_of_assembly.png)
12. Choose custom layout ![](12_custom_layout.png)
13. Do not include title or border ![](13_do_not_include_border_or_title_block.png)
14. Be sure the scale is 1:1 or your parts won't be the correct size. ![](14_drawing_settings.png)
15. Depending on the size of what you are cutting, the paper might be undersized. ![](15_sheet_too_small.png)
We need our sheet size to match the size of our stock material.

17. Open the sheets menu ![](16_sheets_menu.png)
17. Open the properties of the sheet ![](17_open_sheet_properties.png)
18. Choose **Custom** in the format drop down ![](18_custom_format.png)
19. Set the sheet size to match your stock material. The max size for the Laser Cutter is 24" wide by 18" tall. ![](19_sheet_size.png)
20. Be sure the parts are fully contained on the sheet ![](20_parts_on_sheet.png)
21. Export the drawing ![](21_export_drawing.png)
22. Be sure to select SVG as your output format ![](22_export_settings.png)

The SVG file can be cut with the laser cutter. The Laser Cutter Intro guide describes the cutting process in detail.

32. [Next Steps](guides/laser-cutter-intro/#preparing-the-file)