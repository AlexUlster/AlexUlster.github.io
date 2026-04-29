---
title: "Project 1"
layout: single
permalink: /projects/
sidebar:
  title: "Projects"
  nav:
    - projects

cards:
  - title: "Overview"
    image: /assets/images/Placeholder.jpg
    text: "Explain what the project is, the main goal, and what the player or user does."

  - title: "Development"
    image: /assets/images/Placeholder.jpg
    text: "Talk about how the project was made, what changed during development, and what you improved."

  - title: "Main System"
    image: /assets/images/Placeholder.jpg
    text: "Break down an important system, such as combat, enemy AI, UI, mechanics, or level design."
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

## Project Breakdown

<div style="height: 20px;"></div>

{% include video id="oYdRzQwxtAc" %}

{% include project-cards.html cards=page.cards %}

</div>
