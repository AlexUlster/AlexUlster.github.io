---
title: "Project 1"
layout: single
permalink: /projects/projects-pro1/
sidebar:
  title: "Projects"
  nav:
    - projects

cards:
  - title: "Overview"
    image: /assets/images/Placeholder.jpg
    text: "Explain what the project is, the main goal, and what the player or user does."
    tags: ["Game Design", "Unity"]

  - title: "Development"
    image: /assets/images/Placeholder.jpg
    text: "Talk about how the project was made, what changed during development, and what you improved."
    tags: ["Development", "C#"]

  - title: "Main System"
    image: /assets/images/Placeholder.jpg
    text: "Break down an important system, such as combat, enemy AI, UI, mechanics, or level design."
    tags: ["Systems", "Gameplay"]
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

## Here's a list of skills that I have acquired over the course of my game development journey!

{% include video id="YOUR_VIDEO_ID_HERE" %}

{% include project-cards.html cards=page.cards %}

</div>
