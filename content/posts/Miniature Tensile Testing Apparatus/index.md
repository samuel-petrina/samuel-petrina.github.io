---
title: "Miniature Tensile Testing Apparatus"
date: 2022-09-05
tags: ['Solidworks', 'FEA', 'ANSYS', 'DFM']
---

{{< figure src="tensile_rig_rendering.jpg" caption="Rendering of final design done in Solidworks Visualizer" >}}

Material selection for use in the nuclear field provides a unique set of constraints and challenges. Materials are under high stress at elevated temperatures while also being subject to radiation damage. These challenges require a unique field of research to make effective material selection choices. One technology that allows for the observation of a material’s microstructure is x-ray diffraction (XRD). To complement the XRD machine being purchased at Queen’s University, a miniature tensile stage suitable for use inside the XRD machine was needed. I was tasked with designing a suitable tensile stage while working as a summer research assistant.

{{< figure src="tensile_rig_isometric.png" caption="Solidworks model of final design" >}}

The primary challenges of the project were the constraints imposed by the XRD machine. The goniometer that will be used with the XRD machine has a maximum mass limit of 1 kg which defines the mass constraint for the project. To allow for elevated temperature testing, we decided a vacuum chamber is needed to prevent oxidization of the sample. This imposed a size constraint that made the packaging of the system particularly challenging. To prevent the overall length of the device from being too large, we decided the lead screw needed to be placed under the sample and the stepper motor must be placed to the side. This led to the atypical layout of the tensile testing stage.

{{< figure src="tensile_rig_thermal_fea.png" caption="Thermal analysis results in ANSYS. Only parts relevant to the heating system are included" >}}

To replicate the high-temperature environment seen in a nuclear reactor, a heating system was needed. This needed to be accomplished using resistive heating through the sample as heat transfer through the air is impossible in a vacuum. Because no heat loss will occur through convective cooling, the system needed a water-cooling system. This is done using channels directly through the sample jaws preventing heat from reaching any sensitive components including the loadcell, the LVDT, or the stepper motor. I used ANSYS thermal analysis to predict the required current through the sample to reach the desired temperatures and the heat flow from the sample to the jaws.

{{< figure src="tensile_rig_defeatured.png" caption="Defeatured CAD model used for FEA" >}}

To ensure the load frame was adequately stiff to produce accurate results, I set up up a detailed FEA model for the design. I created a defeatured configuration of the assembly in Solidworks which allowed me to easily export a simplified CAD file for use in ANSYS. For elements of the design that would be challenging to mesh such as the loadcell and the lead screw, I replaced them with equivalently stiff spring elements in ANSYS.

{{< figure src="tensile_rig_structural_fea.png" caption="Loadframe stiffness FEA results" >}}