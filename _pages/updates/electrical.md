---
title         : "Summer 2022: Electrical"
permalink     : /updates/electrical
---

In terms of electrical work, our tasks this summer generally fell into two categories. Our effort was divided between adding sensor capability and reworking existing wiring to improve functionality.

## Sensing

Early in the summer, the electrical priority was to hook up and interface with the Blue Robotics temperature and pressure sensors, which had already been physically installed in the computer tube. This process was relatively straightforward (apart from our temperature sensor being temperamental on test day), and these sensors allowed us to actually collect data and operate in a control loop.

The next sensing project was to start integrating the dissolved oxygen and in-house chlorophyll sensors in the second tube into our Jetson. After talking with the group who designed that tube, it became apparent that integration would take time and energy that our electrical team could not devote to it, as we were pushing hard to get the internals rewired before testing could take place. However, if it weren't for that delay, I anticipate it wouldn't have been out of the question to get those sensors connected and functional.

## Rework

Speaking of the electrical rework that delayed the sensor additions, it occurred for a few reasons. A few weeks before the end of the research period, we did some digging into the existing wiring to think about how we could improve the speeds on the thrusters, since they could barely even move the robot in the pool.

As we picked apart the electrical board, we found more shortcomings. First, we realized we needed a capacitor to create a clean power circuit for the Jetson and other sensitive electronics. Next, we realized that the Blue Robotics switch controlling power to the entire robot was limited to 5A, hence the paltry 1A that we were sending to each thruster.

After a lot of thinking and design work, things breaking, and soldering, we completed a wiring rework that includes:

- 18000 micro Farad capacitor for clean power
- relay (controlled by magnetic switch) to power on/off ESCs
- LED to display ESC power status
- terminal bus bars for +13.2V, 5V, 3.3V, GND, and ESCs (switched 13.2V)
- Blue Robotics switch used to power 5V and 3.3V, not thrusters

As a result of this rework, we are now pushing 4A to each thruster, which made an enormous difference. In addition, we have clean power and distinct terminals for various voltages. The magnetic switch for the ESC relay also functions as an external E-stop for thrusters.
