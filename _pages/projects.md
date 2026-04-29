---
title: "Project 1"
layout: single
permalink: /projects/
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

Project 1: Pinata Puncher!

<div style="height: 20px;"></div>

Pinata puncher is a fast paced, 3D, arcade style game where the objective is to punch as many pinatas as you can in one minute and compete with your friends to get the highest score! This was made during the first semester at university.

<div style="height: 20px;"></div>

{% include video id="vPuZRjlojW0" %}

{% include project-cards.html cards=page.cards %}

</div>
