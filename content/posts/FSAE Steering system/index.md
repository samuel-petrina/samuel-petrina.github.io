---
title: "FSAE Steering System"
date: 2023-02-17
tags: ['Solidworks', 'FSAE', 'Ackermann']
---

One particularly challenging subsystem of an FSAE car is the steering system. The primary reason for the difficulty is how close the front wheels are to the steering wheel. In a street car and most open-wheeled vehicles for that matter, the front wheels are well in front of the steering wheel meaning the steering rack and the steering wheel can be connected with a few universal joints. The classic FSAE solution in the past was to place the steering rack in-line with the upper control arm. This meant the steering column could be devoid of universal joints however this had the unfortunate consequence of placing the steering rack above the driver's lower legs. This earned the design its nickname of the "shin-breaker" for obvious reasons.

{{< figure src="steering_column_closeup.JPG"  caption="Adjustable pillow block for bushing">}}

To resolve this safety issue, SAE implemented the chassis cockpit template rule that effectively mandates that the steering is on the floor of the vehicle. Because the steering column needs to traverse a nearly 90-degree angle in such a short distance, steering geometry compromises are often made. This year our team decided to conquer this problem head-on. Our solution was to replace the universal joints with a single right-angle bevel gearbox. This enabled us to place both the steering rack and steering wheel exactly where we wanted them.

{{< figure src="steering_rack_mount.JPG"  caption="Steering rack mounts made with HSS">}}

The primary element of our subsystem was the Zero-Max C156806 gearbox. I chose this unit due to its exceptionally low backlash and its size which enabled it to skirt the cockpit template rules that restrict the steering column size. The next element of the design that I was concerned about was ensuring the gearbox didn't bind due to shaft misalignment. We planned for this in two ways. Where the gearbox was mounted, I designed a bracket that would allow us to shim it into alignment if needed (this proved not to be required). To compensate for any misalignment of the horizontal shaft, we designed a custom bearing block that uses a large, spherical bearing. Additionally, the bearing block mount using slotted holes allows for positional adjustment.

{{< figure src="steering_system.JPG"  caption="Steering column system">}}

We were nervous during the jigging process that the system would move freely, however, the assembly process all went very smoothly. I am very happy with the outcome of this project for two reasons. Firstly, we were able to position the steering rack as needed to accomplish the range of steering that we desired. Secondly, the design is exceptionally easy to implement for future cars being built which should reduce the workload of the team.

