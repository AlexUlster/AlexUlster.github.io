---
title: "Project 1"
layout: default
permalink: /projects/projects-pro1/
---

<style>
  .project-wrapper {
    display: flex;
    gap: 2rem;
    max-width: 1180px;
    width: 100%;
    margin: 0 auto;
    padding: 1rem;
    box-sizing: border-box;
  }

  .project-sidebar {
    width: 180px;
    flex-shrink: 0;
  }

  .project-sidebar a {
    display: block;
    padding: 0.7rem 0;
    color: #555;
    text-decoration: none;
    border-bottom: 1px solid #eee;
  }

  .project-sidebar a:hover {
    color: #f9b248;
  }

  .project-content {
    flex: 1;
    min-width: 0;
  }

  .project-title {
    font-size: 2.4rem;
    margin-bottom: 1.5rem;
  }

  .video-container iframe {
    width: 100%;
    aspect-ratio: 16 / 9;
    border: none;
    border-radius: 14px;
  }

  .section {
    margin: 3rem 0;
  }

  .section p {
    color: #666;
    line-height: 1.7;
  }

  .orange-line {
    width: 60px;
    height: 4px;
    background: #f9b248;
    border-radius: 999px;
    margin-bottom: 0.8rem;
  }

  .overview,
  .image-row,
  .two-col {
    display: grid;
    grid-template-columns: 1fr 1fr;
    gap: 2rem;
  }

  img {
    max-width: 100%;
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
    width: 300px;
    height: 200px;
    object-fit: cover;
    flex-shrink: 0;
  }

  @keyframes scrollGallery {
    100% {
      transform: translateX(-50%);
    }
  }

  @media (max-width: 800px) {
    .project-wrapper {
      flex-direction: column;
    }

    .project-sidebar {
      width: 100%;
    }

    .overview,
    .image-row,
    .two-col {
      grid-template-columns: 1fr;
    }
  }
</style>

<div class="project-wrapper">

  <aside class="project-sidebar">
    <h3>Projects</h3>
    <a href="/projects/projects-pro1/">Project 1</a>
    <a href="/projects/projects-pro2/">Project 2</a>
    <a href="/projects/projects-pro3/">Project 3</a>
  </aside>

  <main class="project-content">

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

  </main>

</div>
