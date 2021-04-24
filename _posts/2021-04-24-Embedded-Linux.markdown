---
layout: post
title: "Embedded Linux at Stanley"
date: 2021-04-24 14:45:00 -0700
author: Tim
categories: linux
---

I worked at Stanley for one intense year. I was hired to help bring a new
telemetry system for very large hydraulic machines to fruition. This
opportunity was extremely appealing to me because it combined many of the
things I love most

1. Building something new from the ground up
2. The freedom to be creative
3. Utilize off-the-shelf hardware, but customize where necessary
4. Embedded Linux + Python
5. Impact! I got to deploy these systems all over the world as soon we got
   prototypes ready.

The machines this system was targeting initially was huge industrial hydraulic
shears. We would measure hydraulic temperature and pressure as well as the GPS
location of the machine and any other telemetry we could get.

![Sensors](/assets/can_sensors.jpeg){:width="80%"}
_CAN bus pressure and temperature sensors_

This is the largest shear Stanley produced at the time.
![HUGE Machine](/assets/big_shear.jpeg){:width="80%"}
_Human for scale_

The environment that the system had to work in was brutal, but the system
worked really well.

The initial computer that was tested didn't stand up to the harsh environment,
so I spent some time debugging broken hardware.

![Broken PCB Mount](/assets/broken_pcb_mount.jpeg){:width="80%"}

We ended up choosing a single board computer (SBC) that was better designed and
was a very rugged little computer. It was very rare, but sometimes even they
would end up with component failures.

![HED Component Failure](/assets/hed_sheared_cap.jpeg){:width="80%"}
_Sheared capacitor_

The wire harness was well documented and I spent some time making
custom development harnesses so we didn't have to pay extreme prices for ones
made by the manufacturer. Adafruit always has the right parts for the job.

![HED Custom Harness](/assets/hed_custom_harness.jpeg){:width="80%"}

Since the computers had cell modems in them we went through a *lot* of SIM
cards during development and field trials.

![SIM Cards](/assets/so_many_sims.jpeg){:width="80%"}

When we were ready to move into production I developed a system that would
automate the entire process as much as possible. I used a Raspberry Pi, some
relays, cell modem network, and a small Pelican case. The box would sit on an
isolated part of the manufacturing plant, and an operator would download the
latest Linux firmware, program all the CAN sensors for the given machine the
were going on. I also wrote some custom code to print out labels for the
sensors, the user manual, and the installation kit.

![Label Printer](/assets/sensor_with_printouts.jpeg){:width="80%"}
_Various sizes of printouts depending on where they were used_

It was important that the serial numbers of every component was captured so
that if one was destroyed in the field we'd be able to trace it's history.

I had so much fun on this project. Getting to see sensor data plots flow into
our cloud data collection system in nearly real time was extremely cool. We had
machines all over the country and several in Canada and in Europe pumping in
data all hours of the day and night.
