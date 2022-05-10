---
title: Toolbox Foam Cutouts
description: How to Make precise cutouts for toolbox organization 
# weight: 40
---

01. Start by making a rough layout
{{< img "01_rough_layout.jpg" "400" >}}


02. Take photos of each of the tools, ensure you have plenty of contrast
{{< columns >}} 
{{< img "02_deadblow_lg.jpg" >}}
<--->
{{< img "02_deadblow_sm.jpg" >}}
<--->
{{< img "02_hammer.jpg" >}}
<--->
{{< img "02_mallet.jpg" >}}
{{< /columns >}}

03. Measure the longest axis of each tool so we can properly scale the images later
{{< img "03_length.jpg" "400" >}}

04. To remove the background, open image in paint3d
{{< img "04_open_in_paint3d.png" "400" >}}

05. Use the Magic Select tool, drag the handles to remove as much background as possible
{{< img "05_shrink_to_solid_bg.png" "400" >}}

06. If you need to refine the selection, Use the Pencil and Eraser to mark parts to keep and parts to remove respectively.
{{< img "06_use_pencil_eraser_to_refine.png" "400" >}}

07. Copy the tool selection and paste in Inkscape. Repeat for all tools, create a layout matching your rough layout from step 1.
{{< img "07_layout_in_inkscape.svg" "400" >}}

08. Use the Width and Height toolbar in Inkscape to ensure your tool is the proper size using the measurements from earlier. Be sure to click the lock icon to ensure the with and height aspect ratio is maintained.
{{< img "08a_resize.png" >}}

08. Use Inkscape's bitmap trace function to convert the tools to vector paths.
{{< img "08_bitmap_trace_menu.png" "400">}}

We've found that the Brightness cutoff with a threshold of .92 or higher works well. If you go too high the results are not as good.
{{< img "08_bitmap_trace_dialog.png" "400">}}

Once you have traced each image, it is safe to delete the original image.

09. The trace tool may leave sharp edges or other imperfections that we need to remove. We'll simplify the generated path to make it easier to work with. Select each tool outline and use the simplify option.
{{< img "09_simplify_menu.png" "400">}}

{{< img "09_simplify.svg" "400" >}}

10. To cleanup any last imperfections, zoom in on each tool and double click. Now we can edit the nodes on the path. Select and delete any that should not be cut. Simplify doesn't always do exactly what we want, but you can manually adjust the nodes. We've found making the path transparent allows one to see the tool image below and adjust if needed.

{{< img "10_cleanup_shoing_nodes.png" "400">}}
Final Result:
{{< img "10_cleanup_traces.svg" "400" >}}

11. We added slots to make it easier to get the tools out.

Use the rectangle tool to create a rectangle across a convenient area to grasp the tool, without compromising the foam's ability to hold the tool.
{{< img "11_rectangle_tool.png" "400">}}
{{< img "11_rectangle.svg" "400">}}

12. We added a chamfer to the rectangle for astethic reasons.
{{< img "11_path_effect_chamfer.png" "400">}}
{{< img "12_rounded_rectangle.svg" "400">}}

13. Combine the individual paths into a single path using the union tool
{{< img "13_union_paths.png" "400">}}

14. Remove fill for cutting
- Make sure the path is selected, then
- From the `Object` menu choose  `Fill and Stroke`
- Choose `No paint`
{{< img "14_choose_no_fill.png" "400" >}}

15. For our Epilog laser we need a stroke width of .001" for cutting
- From the `Stroke Style` tab change the width unit to `in` and change the width to `.001`
- At this point it may look like your drawing is missing, but the lines are too thin to render unless you zoom in.
{{< img "14_stroke_width.png" "400">}}

16. Export for cutting
- Choose File > Save As...
- Be sure to choose PDF

17. [Cut it!](/guides/laser-cutter-intro/#preparing-the-file)