---
layout: post
title: "Laser Tube Alignment"
date: 2014-03-10 20:55:00 -0800
author: Tim
categories: laser
---

It turns out there is a trick to aligning the laser tube and all of the
mirrors. I mention it immediately because I spent a week of evenings attempting
to align all of the various pieces. The process was very frustrating because
without the trick, it's all but impossible to get right. The trick isn't even a
trick at all, but a piece of critical information that should be clearly
explained right from the beginning in any laser alignment manual.  These
machines have two active axes, X and Y. For each axis there are two extreme
positions that some call near and far fields. Near is the position where two
mirrors on a given axis are closest to each other. Far is where two mirrors on
a given axis are farthest from each other. Each mirror has adjustment screws
which allow one to aim the reflected beam up, down, left and right. The tube
mounts also have similar adjustments screws. The purpose of the alignment
process is to make it so that the beam hits the center of the focus lens no
matter where it is in the X-Y plane.  The trick is: one must adjust a different
element for near and far fields. For example, to align the near field on mirror
\#2 you'd adjust the tube, and to align the far field on mirror \#2 you'd adjust
mirror \#1, as shown in the following two diagrams.


![Near Field](/assets/near_2.png){:width="60%"}
![Far Field](/assets/far_2.png){:width="60%"}

Similarly, to align the near and far fields on mirror \#3 you'd adjust mirror \#1
and \#2 respectively.

![Near Field](/assets/near_3.png){:width="60%"}
![Far Field](/assets/far_3.png){:width="60%"}

So, there it is. The simple, yet critical piece of information that allowed me
to be successful in aligning the laser beam. Everything is easy once you know
how I suppose.

## Power

There are four "twist" switches on the front panel of the machine. One is for
powering the stepper driver system that controls the axes. One provides power
to the tube. The other two are switches for two two-prong outlets on the back
of the machine. Those are meant for the air and water pumps.

## Initial Tube Alignment

Aligning the tube initially consists of aiming it so that it is pointed
directly at the center of mirror \#1. The manual says to put a couple layers of
masking tape in front of the mirror and pulse the laser so that it makes a
small burn mark. The mirrors mounts have a metal plate with a circular hole in
it that is at a 45 degree angle to the mirror, which is a convenient place to
stick some tape.

![Mirror Mount](/assets/mirror_mount.jpg){:width="60%"}
![Burned Tape](/assets/burned_tape.jpg){:width="60%"}

The tape immediately caught fire! A nice tall flame burned as I frantically ran
over to blow it out. So, don't use blue painters masking tape. Turns out it's
pretty flammable.  Next, I actually followed the instructions and stuck two
layers of plain old masking tape to the mirror mount. I also decided that 40%
was too much power, so I backed it off to 20%. Much better! A bright flash,
smaller flame, a nice ring of smoke and a burn spot on the tape.

## Tube Adjustments, WTF?

Getting the beam to hit the center of mirror \#1 didn't require much adjustment
to the tube. It hit the center after a few slight adjustments.

It's important to only make minor adjustments as you go along. Each little move
at one end of the beam makes a large change at the other end.

Now, I was ready to move on to mirror \#2. First I put two layers of masking
tape on the plate in front of mirror \#2, moved the Y-axis to the near field
position and pulsed the laser again. The beam was off center, so according to
my near field adjustment procedure, I attempted to adjust the mirror tube some
more.

Adjusting the tube wasn't as easy as it should have been. In fact, it was a
freaking nightmare. The little plastic adjustment screws, under the yoke that
supported the tube, were getting wedged into shallow holes that were drilled
into the yoke. Tightening the screws to raise either side of the yoke would
cause erratic movement as the screw would bind up and then spring out of the
divots in the hole. It's a pretty messed up system, and frankly I'm not sure
how it ever works for anyone except by sheer luck. The crazy thing is that it
appears to be done that way by design. The holes in the yoke were drilled on
purpose.

The solution was to get rid of those holes so the adjustment screws wouldn't
bind up inside them. I put some epoxy into the holes, smoothed it out, covered
the holes in masking tape so the epoxy would stay put and let them dry over
night. The next morning I sanded off any rough edges so that the yoke was
completely smooth. Now the adjustment screws do exactly what I expected them to
do in the first place. They raise and lower each side independently and
smoothly.

![Fixed Yoke](/assets/fixed_yoke.jpg){:width="60%"}

Once the beam was hitting the \#2 mirror near field center, I moved the Y-axis
to the far field position and aimed the beam with the adjustment screws on
mirror \#1. Same routine for mirror \#3. Adjust for near field by aiming mirror
\#1. Adjust for far field by aiming mirror \#2.

I put a new stack of tape on mirror \#3 and pulsed the laser briefly at all four
corners of the table. The result was a single burn mark on the tape, right in
the center of the circle. Woot!

![Fixed Yoke](/assets/mirror3_aligned_burn_mark.jpg){:width="60%"}
