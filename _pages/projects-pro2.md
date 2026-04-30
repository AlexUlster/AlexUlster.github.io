---
title: "Project 2"
layout: single
permalink: /projects/projects-pro2/
sidebar:
  title: "Projects"
  nav:
    - projects

cards:
  - title: "Gameplay"
    image: /assets/images/JG1.png
    text: "The main concept of the game is that the player needs to press the correct gamepad button to jump. This gets really challenging becuase the jump blocks are randomised and change on the fly, which puts the player's reaction time and coordination to the test! Additionally there are traps, spikes and pits scattered over the levels to add more challenge."

  - title: "Design"
    image: /assets/images/JG2.png
    text: "The tielset I used was a really useful asset downloaded from itch.io, however I designed the levels, character, jump blocks, cutscenes, animations, lighting and more by myself in order to tailor this asset to my needs. In my opinion it turned out looking really nice!"

  - title: "Programming"
    image: /assets/images/JG3.png
    text: "There are a lot of scripts being used to make this demo work. The main systems are really the random spawning jump blocks, gamepad input detection, scene loading, transition and cutscene management, particle spawning and quite a bit more. This was definitely a techncal challenge as it was one of the first times expreimenting with gamepad inputs in Unity!"
---

<style>
  .project-scale {
    width: 150%;
  }

  @media (max-width: 768px) {
    .project-scale {
      width: 100%;
    }
  }
</style>

<div class="project-scale">

Project 2: Jump Game Demo!

<div style="height: 20px;"></div>

Jump Game is a 2D, level based jumping game. It uses gamepad controls to make the player jump depending on the type of jump block the player is attached to. I made this during the first semester at university!

<div style="height: 20px;"></div>

{% include video id="MPFnFY2fxZY" %}

{% include project-cards.html cards=page.cards %}

</div>
