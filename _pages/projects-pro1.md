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
  /* widen content but respect theme */
  .page__content {
    max-width: 1100px;
  }

  .project-title {
    font-size: 2.6rem;
    margin-bottom: 1.5rem;
  }

  .video-container {
    margin-bottom: 3rem;
  }

  .video-container iframe,
  .video-container video {
    width: 100%;
    aspect-ratio: 16 / 9;
    border-radius: 14px;
    border: none;
    box-shadow: 0 6px 18px rgba(0,0,0,0.15);
  }

  .section {
    margin-bottom: 3.5rem;
  }

  .section h2 {
    font-size: 1.8rem;
    margin-bottom: 0.7rem;
  }

  .section p {
    color: #666;
    line-height: 1.7;
    font-size: 1rem;
    max-width: 800px;
  }

  .orange-line {
    width: 60px;
    height: 4px;
    background: #f9b248;
    margin-bottom: 0.8rem;
    border-radius: 999px;
  }

  .overview {
    display: grid;
    grid-template-columns: 1fr 1fr;
    gap: 2rem;
    align-items: center;
  }

  .overview img {
    width: 100%;
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

  .gallery-track:hover {
    animation-play-state: paused;
  }

  .gallery-track img {
    width: 300px;
    height: 200px;
    object-fit: cover;
    flex-shrink: 0;
  }

  @keyframes scrollGallery {
    0% { transform: translateX(0); }
    100% { transform: translateX(-50%); }
  }

  .two-col {
    display: grid;
    grid-template-columns: 1fr 1fr;
    gap: 2rem;
  }

  .image-row {
    display: grid;
    grid-template-columns: 1fr 1fr;
    gap: 2rem;
    align-items: center;
  }

  .image-row img {
    width: 100%;
    border-radius: 14px;
  }

  @media (max-width: 768px) {
    .overview,
    .two-col,
    .image-row {
      grid-template-columns: 1fr;
    }
  }
</style>

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
      Keep this as your main introduction.
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
      Talk about how the project was made. Planning, iteration, problems you solved,
      and how things improved over time.
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
      Break down your most important system (combat, AI, mechanics, etc).
      This is where you show technical understanding.
    </p>
  </div>
</div>
