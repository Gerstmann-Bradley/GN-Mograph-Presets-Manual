Proximity Falloff
=============
Description
------------
This node generates a single/multiple spherical falloff. Upon evaluation, vectors close to the center of the falloff will obtain the Maximum Value (Default= 1), and those far from the center will obtain the Minimum Value (Default= 0).
The core node used in this presets is "Geometry Proximity", so that falloff generation can be done by vertices/Points from a "Geometry" as well.

Inputs
-------------
- **Custom Vector** - Corresponds to the "Source Position" of "Geometry Proximity". By default it uses "Position" Attribute for evaluation.
- **Obj/Mesh** - When Checked, the presets uses "Object Mode", in which you can use Object in the viewport to control the location and scale of your falloff. If it's un-checked, the preset is in "Mesh Mode", in which you are using Geometry from the node tree to control your falloff. Note that Mesh Mode only supports "Point" setting in Geometry Proximity node.
- **Object** - The object used in Object Mode
- **Mesh** - The mesh used in Mesh Mode.
- **Location Offset** - Offset of Vector in addition to the vector imposed by Object in Object Mode / Mesh Points in Mesh Mode.
- **Scale Offset** - Offset of Scale in addition to the vector imposed by Object in Object Mode / Mesh Points in Mesh Mode. Note that Mesh Points doesn't contain scale, thus in order to make "Mesh Mode" work, "Scale Offset>0" is required.
- **Falloff Animation** - A slider goes from 0-1, Meaning the falloff value goes from "Minimum (Default= 0)" to "Maximum (Default= 1)" following the gradient assigned by Falloff.
- **Min** - Minimal Output of Falloff
- **Max** - Maximal Output of Falloff
