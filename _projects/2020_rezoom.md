---
layout: page
title: Project ReZoom
description: Developing Autonomous Electric Scooters
img: assets/img/2020_rezoom_mi.jpg
importance: 7
category: work
---

Demand for autonomous, self-driving modes of transportation are becoming increasingly popular as our society advances towards more efficient ways to get around. Despite their promise of sustainable, accessible, and equitable transportation, shared electric scooters clutter city sidewalks and landscapes. This public nuisance causes city planners to limit the number of shared operators and the size of their scooter fleets, which in turn reduces revenue and diminishes the potential benefits of dockless scooters.

<div class="row justify-content-sm-center">
    <div class="col-sm-5 mt-3 mt-md-0">
        {% include figure.html path="assets/img/2020_rezoom_clutter1.png" title="Scooter Clutter" class="img-fluid rounded z-depth-1" %}
    </div>
    <div class="col-sm-8 mt-3 mt-md-0">
        {% include figure.html path="assets/img/2020_rezoom_clutter2.png" title="Scooter Clutter" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    Electric scooters left on sidewalk are a public nuisance.
</div>


Also, there are large daily operating expenses with the rebalancing of conventional scooters using cars and vans. Not only is rebalancing very expensive, but it ends up undoing a lot of the environmental benefit of shared electric scooters in terms of greenhouse gas emissions. Instead, with our planned autonomous electric scooter, the scooter can reposition itself, albeit over short distances. Additionally, a rider using a self-driving e-scooter fleet is less likely to find a scooter without sufficient battery charge. 

I have been a part of this project, named ReZoom, since June 2021. During this time, I have worked on three generations of our self-driving scooter prototypes, which are OEM scooters fitted with additional hardware. 


<div class="row justify-content-sm-center">
    <div class="col-sm-5 mt-3 mt-md-0">
        {% include figure.html path="assets/img/2020_rezoom_mi_hover.jpg" title="Hover and Mi Scooter" class="img-fluid rounded z-depth-1" %}
    </div>
    <div class="col-sm-7 mt-3 mt-md-0">
        {% include figure.html path="assets/img/2020_rezoom_mi.jpg" title="Mi Scooter" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    [Left] The taller, version 2 of the ReZoom scooter alongside version 1. [Right] The version 2 scooter operated outdoors.
</div>

<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.html path="assets/img/2020_rezoom_hiboy.png" title="Hiboy Scooter" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    The upcoming version 3 of our autonomous scooter fleet.
</div>

From a technology standpoint, most self-driving vehicles are either large and operate over larger distances (think self-driving cars and trucks) or are small and operate indoors. Self-driving electric scooters present a novel challenge because of their small form-factor, small battery capacity and low unit costs. An autonomous e-scooter is required to travel along roads, follow traffic signs, and avoid pedestrians, just as an autonomous car would.

I have been working on these challenges by adapting open source packages in ROS for the unique constraints that an electric scooter poses. My role in the team is to develop the state estimate, develop waypoint based path planning, testing various approaches for VIO, navigation, sensor filtering, and to perform system integration while resolving any software and electrical issues that arise. 

Presently, the scooter is capable of accepting a list of GPS waypoints and travel down that path autonomously. I have been able to demonstrate 230 meters of autonomous travel of the scooter along campus roads. However, this relies on blind state estimation (only GPS, Wheel and IMU data; no VIO) and obstacle avoidance using stereo depth only. We are constantly working on improving the scooter's capabilities, and there is still a lot to do!
