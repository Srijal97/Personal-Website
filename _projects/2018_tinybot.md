---
layout: page
title: TinyBot
description: A very tiny (~ 10x10x10 mm) wireless remote-controlled car.
img: assets/img/2019_tinybot_thumb.jpeg
importance: 3
category: fun
---


It started out with a claim on the title of “smallest robot” in a Reddit post [image below]. It used the ESP8266 as the controller, motor driver boards on the sides, a LiPo battery and small stepper motors at the bottom. Pretty impressive, but I decided to try and do better.

<div style="text-align: center">
    <div class="row">
        <div class="col-sm mt-3 mt-md-0">
            {% include figure.html path="assets/img/2019_tinybot_smallest_bot_old.jpg" title="example image" class="img-fluid center rounded z-depth-1" %}
        </div>
    </div>
</div>
<div class="caption">
    The "smallest robot" as claimed by someone in a Reddit post.
</div>



In my design, I used the ESP8285 (ESP-01F) module, which is half the size of the ESP8266 (ESP12) module used above. Along with a custom PCB for the power and 2x motor drivers, the overall dimensions are about 10mm*10mm. 

Tiny stepper motors are used for movement, and a python script running on a PC uses MQTT for communication with the modules. MQTT has been designed with multiple robot communication in mind, and seemed perfect for creating a swarm of multiple such TinyBots! That's what I call them - TinyBots...super creative!


<div class="row justify-content-sm-center">
    <div class="col-sm-8 mt-3 mt-md-0">
        {% include figure.html path="assets/img/2019_tinybot_components.jpeg" title="Assembled device" class="img-fluid rounded z-depth-1" %}
    </div>
    <div class="col-sm-4 mt-3 mt-md-0">
        {% include figure.html path="assets/img/2019_tinybot_esp_comparison.jpeg" title="Device PCB" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    TinyBot components and ESP-01F vs ESP12 modules size comparison.
</div>

<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.html path="assets/img/2019_tinybot_programmer.jpeg" title="Assembled device" class="img-fluid rounded z-depth-1" %}
    </div>
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.html path="assets/img/2019_tinybot_soldering.jpeg" title="Device PCB" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    [Left] A programming tool had to be hand-crafted for the tiny ESP-01F, [Right] Soldering the PCB with 0201 SMD components. If you look closely, there are two 0201 components between the two switch pins!
</div>


<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.html path="assets/img/2019_tinybot_assembly.jpeg" title="Assembled device" class="img-fluid rounded z-depth-1" %}
    </div>
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.html path="assets/img/2019_tinybot_wired_testing.jpeg" title="Device PCB" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    [Left] Assembling the robot, [Right] Wired testing as I wait for batteries to arrive.
</div>


I had trouble procuring the 10mm LiPo batteries (smallest that can be found online) because of import regulations on lithium batteries in India. Eventually, I did get them but testing showed that the battery voltage quickly dropped when the stepper motors are loaded (drawing higher current), causing the ESP8285 to reset. Shown below is a short video of the bot controlled from my Desktop. 

<iframe width="100%" height="460" src="https://www.youtube.com/embed/FIK_Xq2O9Hg" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>

The C rating of the batteries in such a small package is not sufficient to support the requirements of TinyBot. I don’t see getting better batteries under my budget anytime soon - I am limited by the technology of my time! The current project code and PCB files can be found at [TinyBot on GitHub](https://github.com/Srijal97/TinyBot).
