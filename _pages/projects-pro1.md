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
    transform: scale(2);
    transform-origin: top left;
    width: 80%;
  }

  .project-title {
    font-size: 2rem;
    margin-bottom: 1.5rem;
  }

  .video-container {
    margin-bottom: 2.5rem;
  }

  .video-container iframe {
    width: 100%;
    aspect-ratio: 16 / 9;
    border: none;
    border-radius: 14px;
  }

  .section {
    margin-bottom: 3rem;
  }

  .orange-line {
    width: 60px;
    height: 4px;
    background: #f9b248;
    border-radius: 999px;
    margin-bottom: 0.8rem;
  }

  .overview {
    display: grid;
    grid-template-columns: 1fr 1fr;
    gap: 20px;
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
  }

  .project-scale img {
    width: 100%;
    height: auto;
    border-radius: 14px;
  }

  .scrolling-gallery {
    overflow: hidden;
    border-radius: 14px;
    background: #f9b248;
  }

  .gallery-track {
    display: flex;
    animation: scrollGallery 18s linear infinite;
  }

  .gallery-track img {
    width: 260px;
    height: 170px;
    object-fit: cover;
    flex-shrink: 0;
    border-radius: 0;
  }

  @keyframes scrollGallery {
    0% {
      transform: translateX(0);
    }

    100% {
      transform: translateX(-50%);
    }
  }

  @media (max-width: 768px) {
    .project-scale {
      transform: none;
      width: 100%;
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

  <div class="video-container">
    <iframe 
      src="https://www.youtube.com/embed/YOUR_VIDEO_ID_HERE"
      title="Project Video"
      allowfullscreen>
    </iframe>
  </div>

  <div class="section overview">
    <div>
      <div class="orange-line"></div>
      <h2>Project Overview</h2>
      <p>
        Explain what your project is, what the goal is, and what the user/player does.
      </p>
      <p>
        Mention your role, tools used, and what makes this project interesting.
      </p>
    </div>

    <img src="/assets/images/Placeholder.jpg" alt="Overview image">
  </div>

  <div class="section">
    <div class="orange-line"></div>
    <h2>Image Gallery</h2>

    <div class="scrolling-gallery">
      <div class="gallery-track">
        <img src="/assets/images/Placeholder.jpg">
        <img src="/assets/images/Placeholder.jpg">
        <img src="/assets/images/Placeholder.jpg">
        <img src="/assets/images/Placeholder.jpg">

        <img src="/assets/images/Placeholder.jpg">
        <img src="/assets/images/Placeholder.jpg">
        <img src="/assets/images/Placeholder.jpg">
        <img src="/assets/images/Placeholder.jpg">
      </div>
    </div>
  </div>

  <div class="section two-col">
    <div>
      <div class="orange-line"></div>
      <h2>Development</h2>
      <p>
        Talk about how the project was made, problems you solved, and improvements.
      </p>
    </div>

    <div>
      <div class="orange-line"></div>
      <h2>My Role</h2>
      <p>
        What you specifically worked on: programming, gameplay, UI, animation, etc.
      </p>
    </div>
  </div>

  <div class="section image-row">
    <img src="/assets/images/Placeholder.jpg">

    <div>
      <div class="orange-line"></div>
      <h2>Main System</h2>
      <p>
        Break down your most important system, like combat, AI, or mechanics.
      </p>
    </div>
  </div>

</div>
