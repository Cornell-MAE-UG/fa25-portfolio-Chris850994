---
layout: project
title: Analysis of Functions 
description: Class project with Graphs (10/3/2025)
technologies:
image: ({{ "assets/images/image_actuator.jpg" | relative_url }}){: class="profile-image"}


---


As part of a class project I adressed the problem through developing a triangle within the bounds.  The triangle consists of two static supports and an IMA actuator of inital length 0.2662m between the supports.  Each support was perpendicular to the ground.  I then summed the moment of the system to find the maximum weight.  I found that the weight the structure could support was dependent on the distance of the actuator from the orgin.  Thus, to maximize this distance, the actuator had to be extending to a length roughly equal to the vertical component of the triangle.


This is how I solved the problem:

```python
    Given a triangle of length 1.5m, height .5m, and hypotenuse of 1.58m, taking the moment about point O in the image yields the equation:
    0 = 1.5(w) - r1(36) - (r1+r2)(36)
    where w is weight, r1 is the distance from the orgin to the first support and r2 is the distance from the first support to the second support.
    To maximize the weight supportable, r1+r2 and r1 = ~1.5 (the actuator can't occupy the same space as another support)
    Thus let r1 = 1.48 and r1+r2 = 1.49
    Length of extension of the actuator would be the length required for actuator to reach the maximum height in the bound (0.5m) so length of extension Lo would be 5 - 0.2662 = .2338 m
    Therefore, solving the equation yields
    Length of extension Lo = .2338m
    Total weight w supported = 71.28N
```




