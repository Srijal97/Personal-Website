---
layout: page
title: Project ReZoom
description: Developing Autonomous Electric Scooters
img: assets/img/2020_rezoom_mi_scooter.jpg
importance: 7
category: work
---

Demand for autonomous, self-driving modes of transportation are becoming increasingly popular as our society advances towards more efficient ways to get around. Despite their promise of sustainable, accessible, and equitable transportation, shared electric scooters clutter city sidewalks and landscapes. This public nuisance causes city planners to limit the number of shared operators and the size of their scooter fleets, which in turn reduces revenue and diminishes the potential benefits of dockless scooters.

[Insert image of scooter clutter]

Also, there are large daily operating expenses with the rebalancing of conventional scooters using cars and vans. Not only is rebalancing very expensive, but it ends up undoing a lot of the environmental benefit of shared electric scooters in terms of greenhouse gas emissions. Instead, with our planned autonomous electric scooter, the scooter can reposition itself, albeit over short distances. Additionally, a rider using a self-driving e-scooter fleet is less likely to find a scooter without sufficient battery charge. 

I have been a part of this project, named ReZoom, since June 2021. During this time, I have worked on three generations of our self-driving scooter prototypes, which are OEM scooters fitted with additional hardware. 

[Insert images of all three scooters]

From a technology standpoint, most self-driving vehicles are either large and operate over larger distances (think self-driving cars and trucks) or are small and operate indoors. Self-driving electric scooters present a novel challenge because of their small form-factor, small battery capacity and low unit costs. An autonomous e-scooter is required to travel along roads, follow traffic signs, and avoid pedestrians, just as an autonomous car would.

I have been working on these challenges by adapting open source packages in ROS for the unique constraints that an electric scooter poses. My role in the team is to develop the state estimate, develop waypoint based path planning, testing various approaches for VIO, navigation, sensor filtering, and to perform system integration while resolving any software and electrical issues that arise. 

Presently, the scooter is capable of accepting a list of GPS waypoints and travel down that path autonomously. Below is a video of the scooter travelling a distance of about 230 meters in self-driving mode. 

[Insert video of scooter run through Engineering Drive]

However, this relies on blind state estimation (only GPS, Wheel and IMU data; no VIO) and obstacle avoidance using stereo depth only. We are constantly working on improving the scooter's capabilities, and there is still a lot to do!
