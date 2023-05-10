---
title: "FSAE Control Arms"
date: 2022-12-18
tags: ['FSAE', 'Solidworks', 'MATLAB']
---

{{< figure src="welded_wishbones.jpg"  caption="Wishbones after being tacked on jigging plate, ready to be welded">}}

In previous years, our team has used carbon fiber control arms made by gluing aluminum lugs into the end of carbon tubing. This works quite well for tie-rods and pushrods where the lug is a simple cylindrical part with a tapped hole for rod-end bearings. The lugs for the wishbones however were a complex 4-axis milling job that caused issues for our team. With limited machining experience and one of our machine shop sponsors falling through, we decided to opt for a simpler steel design.

{{< figure src="wishbone_cad.png"  caption="Wishbone CAD in Solidworks. Each wishbone size has its own assembly configuration">}}

The first step in our design process was to calculate suspension loading. I did this by writing a custom MATLAB script that uses matrix math to calculate the control-arm loading in a variety of loading conditions. The script then outputs the maximum compression and tension loading that each member could see. To determine the required tubing, I used another custom MATLAB script. The code takes the inner and outer diameter of the tubing as well as the applied load and material properties then outputs the factor of safety for both buckling and tensile failure.

{{< figure src="tube_end_nuts.jpg"  caption="4130 tubing with tube-end nuts welded for rod-end bearings">}}

For pushrods, tie-rods, toe-rods, and the chassis side of the wishbones, we used weld-in-nuts that allow us to easily thread in rod-end bearings. At the wheel side of the wishbones, we used water-jetted 1/4" chromoly plate into lugs that will slot into our tubing. We sized these lugs based on the required weld bead length that we needed for the applied load. After cutting our tubing to length and welding the tube-end nuts into one side of the tubing we started work on our jigging plate. I carefully laid out our wishbone geometry onto a plate of aluminum based on our CAD in Solidworks. Using 1/4" fasteners, we bolted the wishbones into shape so the welder at our school shop could finish them up. 

{{< figure src="jigging_plate.jpg"  caption="Two wishbones on jigging plate ready for welding">}}