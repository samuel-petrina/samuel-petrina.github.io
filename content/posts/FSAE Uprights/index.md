---
title: "FSAE Uprights"
date: 2022-11-20
tags: ['FSAE','Solidworks', 'FEA', 'ANSYS', 'DFM']
---

{{< figure src="rear_upright.jpg"  caption="Finished rear upright">}}

Because our suspension geometry had changed significantly from our previous car, we needed to design and manufacture new front and rear uprights. Our primary goal for this year's design was manufacturability. For us, this meant ensuring all features can be machined from just two milling machine setups. Our front geometry was similar to the previous design so we had the option to simply modify the old CAD. Unfortunately, because it was designed using lofts and surface modeling, it was frustrating at best to edit the design.

{{< figure src="rear_upright_cad.png"  caption="Rear upright CAD in Solidworks">}}

The material that we used for the uprights was purchased in early 2020 before we were shut down by COVID. This meant that we had to ensure that our design would fit inside the billets that we already had. For the front upright, this mandated the bolt-on tie-rod attachment instead of having an integral clevis. For the rear upright, we integrated the control arm attachment points directly into the upright as opposed to having them bolt on. Removing this bolted connection allowed the design to fit into the existing billet. While designing the component, I focused on maintaining editable CAD. This enabled easier and faster iterations of the design.

{{< figure src="front_upright.jpg"  caption="Finished front upright">}}

To complete FEA on the uprights, we used a remote point load to apply force to the upright at the contact patch of the tire. This meant the moment caused by the radius of the tire was correctly replicated. To constrain the upright, we locked translation in specific directions at each control arm attachment point. This meant that each attachment point would only take load in the direction that was physically possible. For example, a tie-rod can only apply load in-line with itself. Due to a lack of machining experience on our team, we decided to have our school shop help us. In the end, we were happy with our choice to have the professionals do the work when we saw the final product.

{{< figure src="front_upright_cad.png"  caption="Front upright CAD in Solidworks">}}