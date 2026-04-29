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
    image: /assets/images/PP1.png
    text: "Pinata Punchers has a simple gameplay loop. Players have 60 seconds to punch as many pinatas as possible to get a high score. The map includes various routes and secret pathways to allow players to make each runthrough more effecient than the last as they learn the most optmised routes."

  - title: "Design"
    image: /assets/images/Placeholder.jpg
    text: "I made most of the 3D assets myself in Blender / Unity Pro-Builder and created the textures in the image editing software, Krita. I aimed to create a more retro-stylised PS2 style game by pixelating textures and reducing the resolution of the main camera which I thought gave it a nice effect."

  - title: "Programming"
    image: /assets/images/Placeholder.jpg
    text: "The main piece of programming is the random pinata spawner script which handles where the pinatas spawn by referencing random transform positions around the map."
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

Project 2: Jump Game!

<div style="height: 20px;"></div>

Jump Game is a 2D, level based jumping game. It uses gamepad controls to make the player jump depending on the type of jump block the player is attached to.

<div style="height: 20px;"></div>

{% include video id="MPFnFY2fxZY" %}

{% include project-cards.html cards=page.cards %}

</div>
