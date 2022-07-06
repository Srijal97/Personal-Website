---
layout: page
title: Modular Robots
description: Self‐reconfigurable robot modules.
img: assets/img/2017_dtto_main.jpg
importance: 2
category: work
---

Performing well in the e-Yantra Robotics Competition landed me this awesome internship experience in the e-Yantra Summer Internship Programme, 2017. The project I was assigned to was ‘Modular Robots’. The idea behind modular robots is to create an adaptable robot which can transform and change its gait patterns in the best way possible for a given situation.

Based on the [Dtto: Modular Robot by Alberto](https://hackaday.io/project/9976-dtto-explorer-modular-robot), the objective was to recreate the modules to expand its capabilities and to also explore the possibility of it being a theme in future competitions. I had very interesting discussions with Alberto, however the 7-weeks duration for the internship was simple insufficient to explore all that I hoped to achieve.

In all, I created 4 robotic modules with the addition of a laser ToF sensor on one of the module faces. You can see them in action here:

<iframe width="100%" height="460" src="https://www.youtube.com/embed/yvgkiGqmVyg" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>

One of the problems was that the motors used were underpowered as compared to the original Dtto, so the modules struggled to perform complex manoeuvres. This can be noted in the video below:

<iframe width="100%" height="460" src="https://www.youtube.com/embed/xD0Jfdtmo24" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>

A ‘Virtual Dtto’ environment was created in V-REP for simulation of the modules. This ‘Virtual Dtto’ can be directly controlled via bluetooth using a smartphone, exactly like the real Dtto modules, and can be found on our GitHub repository linked below. Also, a scaled up version of the Dtto was created because the tiny motors used in the normal modules were underpowered for most transformations.

Each day of the internship was a treasure of experiences and excitement; with regular workshops, events and also heritage trips. I met with some super awesome people and had great fun having the 3D printer spit out part after part! Thank you e-Yantra for making this possible.

Check out [eYSIP_Modular_Robot on GitHub](https://github.com/Srijal97/eYSIP-2017_Modular-Robot) for a detailed documentation, design files and code.


<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.html path="assets/img/2017_dtto_main.jpg" title="Four completed modules" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    The four completed modules of the Dtto
</div>

<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.html path="assets/img/2017_dtto_inner.jpg" title="Internal components" class="img-fluid rounded z-depth-1" %}
    </div>
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.html path="assets/img/2017_dtto_face.jpg" title="Face with ToF sensor" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    [Left] Module internals, [Right] Module face with laser ToF sensor.
</div>

<div class="row justify-content-sm-center">
    <div class="col-sm-8 mt-3 mt-md-0">
        {% include figure.html path="assets/img/2017_dtto_present.jpg" title="Presentation Day" class="img-fluid rounded z-depth-1" %}
    </div>
    <div class="col-sm-4 mt-3 mt-md-0">
        {% include figure.html path="assets/img/2017_dtto_me.jpg" title="Me" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    [Left] Modules on display during presentation day, [Right] My workspace during the internship. Fun times!
</div>