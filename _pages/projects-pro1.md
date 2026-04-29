---
title: "Project 1"
layout: single
permalink: /projects/projects-pro1/
sidebar:
  title: "Projects"
  nav:
    - projects
---

<style>
  .project-scale {
    width: 150%;
  }

  .project-title {
    font-size: 2rem;
    margin-bottom: 1.5rem;
  }

  /* ONLY scale the video */
  .project-video-scale {
    transform: scale(1.82);
    transform-origin: top left;
    width: 54.95%;
    margin-bottom: 260px;
  }

  .video-container iframe {
    width: 100%;
    aspect-ratio: 16 / 9;
    border: none;
    border-radius: 14px;
  }

  .section {
    margin-bottom: 3.5rem;
  }

  .section h2 {
    margin-bottom: 0.6rem;
  }

  .section p {
    color: #666;
    line-height: 1.7;
  }

  .overview {
    display: grid;
    grid-template-columns: 1fr 1fr;
    gap: 20px;
    align-items: center;
  }

  .two-col {
    display: grid;
    grid-template-columns: 1fr 1fr;
    gap: 20px;
  }

  .image-row {
    display: grid;
    grid-template-columns: 1fr 1fr;
    gap: 20px;
    align-items: center;
  }

  .project-scale img {
    width: 100%;
    height: auto;
    border-radius: 14px;
  }

  @media (max-width: 768px) {
    .project-video-scale {
      transform: none;
      width: 100%;
      margin-bottom: 2rem;
    }

    .overview,
    .two-col,
    .image-row {
      grid-template-columns: 1fr;
    }
  }
</style>

<div class="project-scale">

  <h1 class="project-title">Project 1</h1>

  <!-- VIDEO -->
  <div class="project-video-scale">
    <div class="video-container">
      <iframe 
        src="https://www.youtube.com/embed/YOUR_VIDEO_ID_HERE"
        title="Project Video"
        allowfullscreen>
      </iframe>
    </div>
  </div>

  <!-- OVERVIEW -->
  <div class="section overview">
    <div>
      <h2>Project Overview</h2>
      <p>
        Explain what your project is, what the goal is, and what the player does.
      </p>
      <p>
        Mention your role, tools used, and what makes this project interesting.
      </p>
    </div>

    <img src="/assets/images/Placeholder.jpg" alt="Overview image">
  </div>

  <!-- TEXT SECTIONS -->
  <div class="section two-col">
    <div>
      <h2>Development</h2>
      <p>
        Talk about how the project was made, problems you solved, and improvements.
      </p>
    </div>

    <div>
      <h2>My Role</h2>
      <p>
        What you specifically worked on: programming, gameplay, UI, animation, etc.
      </p>
    </div>
  </div>

  <!-- FEATURE -->
  <div class="section image-row">
    <img src="/assets/images/Placeholder.jpg">

    <div>
      <h2>Main System</h2>
      <p>
        Break down your most important system like combat, AI, or mechanics.
      </p>
    </div>
  </div>

</div>
