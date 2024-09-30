---
title: "FSAE Anti-roll Bar"
date: 2023-03-23
tags: ['Solidworks']
---

{{< figure src="ARB.JPG"  caption="ARB before powder coat">}}

Overly complex anti-roll bar designs seem to be a theme in FSAE (our team included). This year, the main way we reduced complexity was by placing the bushings on the outside of the arms. This meant that the arms and shaft could be a single welded assembly. Previous designs used a hex connection between the arms and the shaft which was bound to fail, have an excessive backlash, or just be a pain to manufacture at minimum. Our final design was a simple turned shaft with 4 water-jet pieces. Instead of complex titanium blades for stiffness adjustments, we simply made three bars, with three mounting holes giving 9 total settings.

{{< figure src="ARB_arms.JPG"  caption="Closeup of arms">}}

The second way this design made our lives easier was by making the structural analysis quite straight-forwards. For the shaft analysis, I prepared a simple spreadsheet that would output roll-stiffness contributions and factor-of-safety for the anti-roll bar shaft. The arms were validated with some quick beam analysis which showed the deflection is negligable compared to the shaft torsion. Finally, the welds were quite simple to analyze as the entire bead is equidistant from the shaft center line meaning the stress is evenly distributed.

{{< figure src="spreadsheet.png"  caption="Shaft analysis">}}