---
title: "Project 1"
layout: default
permalink: /projects/projects-pro1/
---

<style>
  .project-layout {
    display: grid;
    grid-template-columns: 220px 1fr;
    gap: 3rem;
    max-width: 1400px;
    margin: 0 auto;
    padding: 1rem;
  }

  .project-sidebar {
    position: sticky;
    top: 2rem;
    align-self: start;
  }

  .project-sidebar h3 {
    margin-bottom: 1rem;
    color: #333;
  }

  .project-sidebar a {
    display: block;
    color: #555;
    text-decoration: none;
    padding: 0.7rem 0;
    border-bottom: 1px solid #eee;
    transition: all 0.3s ease;
  }

  .project-sidebar a:hover {
    color: #f9b248;
    transform: translateX(5px);
  }

  .project-content {
    width: 100%;
  }

  .project-title {
    font-size: 3rem;
    color: #333;
    margin-bottom: 1.5rem;
  }

  .video-container {
    width: 100%;
    margin-bottom: 3rem;
  }

  .video-container iframe,
  .video-container video {
    width: 100%;
    aspect-ratio: 16 / 9;
    border: none;
    border-radius: 16px;
    display: block;
    box-shadow: 0 8px 24px rgba(0,0,0,0.14);
  }

  .section {
    margin-bottom: 4rem;
  }

  .section h2 {
    font-size: 2rem;
    color: #333;
    margin-bottom: 1rem;
  }

  .section p {
    color: #666;
    line-height: 1.8;
    font-size: 1.05rem;
    max-width: 900px;
  }

  .overview-split {
    display: grid;
    grid-template-columns: 1.1fr 0.9fr;
    gap: 2.5rem;
    align-items: center;
  }

  .overview-split img {
    width: 100%;
    border-radius: 16px;
    box-shadow: 0 8px 24px rgba(0,0,0,0.12);
  }

  .orange-line {
    width: 80px;
    height: 5px;
    background: #f9b248;
    border-radius: 99px;
    margin-bottom: 1.2rem;
  }

  .scrolling-gallery {
    overflow: hidden;
    border-radius: 16px;
    background: #f9b248;
    box-shadow: 0 8px 24px rgba(0,0,0,0.12);
  }

  .gallery-track {
    display: flex;
    animation: scrollGallery 18s linear infinite;
  }

  .gallery-track:hover {
    animation-play-state: paused;
  }

  .gallery-track img {
    width: 360px;
    height: 230px;
    object-fit: cover;
    flex-shrink: 0;
  }

  @keyframes scrollGallery {
    0% {
      transform: translateX(0);
    }
    100% {
      transform: translateX(-50%);
    }
  }

  .two-column-text {
    display: grid;
    grid-template-columns: 1fr 1fr;
    gap: 3rem;
  }

  .image-text-row {
    display: grid;
    grid-template-columns: 0.9fr 1.1fr;
    gap: 2.5rem;
    align-items: center;
  }

  .image-text-row img {
    width: 100%;
    border-radius: 16px;
    box-shadow: 0 8px 24px rgba(0,0,0,0.12);
  }

  .big-orange-section {
    background: linear-gradient(135deg, #f9b248 0%, #f79e47 100%);
    margin: 4rem -2rem 0 -2rem;
    padding: 3rem 2rem;
    border-radius: 20px;
    color: white;
  }

  .big-orange-section h2 {
    color: white;
  }

  .big-orange-section p {
    color: white;
    opacity: 0.95;
  }

  @media (max-width: 900px) {
    .project-layout {
      grid-template-columns: 1fr;
    }

    .project-sidebar {
      position: static;
      display: flex;
      gap: 1rem;
      flex-wrap: wrap;
    }

    .project-sidebar h3 {
      width: 100%;
    }

    .overview-split,
    .two-column-text,
    .image-text-row {
      grid-template-columns: 1fr;
    }

    .project-title {
      font-size: 2.3rem;
    }

    .big-orange-section {
      margin: 3rem 0 0 0;
    }
  }
</style>

<div class="project-layout">

  <aside class="project-sidebar">
    <h3>Projects</h3>
    <a href="/projects/projects-pro1/">Project 1</a>
    <a href="/projects/projects-pro2/">Project 2</a>
    <a href="/projects/projects-pro3/">Project 3</a>
  </aside>

  <main class="project-content">

    <h1 class="project-title">Project 1</h1>

    <section class="video-container">
      <iframe 
        src="https://www.youtube.com/embed/YOUR_VIDEO_ID_HERE"
        title="Project 1 Video Demo"
        allowfullscreen>
      </iframe>
    </section>

    <section class="section overview-split">
      <div>
        <div class="orange-line"></div>
        <h2>Project Overview</h2>
        <p>
          This section should introduce the project and explain what it is. Talk about
          the main idea, the genre, and what the player or user is expected to do.
        </p>
        <p>
          You can also mention your role in the project, what tools you used, and the
          main systems or features you personally worked on.
        </p>
      </div>

      <img src="/assets/images/Placeholder.jpg" alt="Project overview image">
    </section>

    <section class="section">
      <div class="orange-line"></div>
      <h2>Image Gallery</h2>

      <div class="scrolling-gallery">
        <div class="gallery-track">
          <img src="/assets/images/Placeholder.jpg" alt="Project screenshot 1">
          <img src="/assets/images/Placeholder.jpg" alt="Project screenshot 2">
          <img src="/assets/images/Placeholder.jpg" alt="Project screenshot 3">
          <img src="/assets/images/Placeholder.jpg" alt="Project screenshot 4">

          <img src="/assets/images/Placeholder.jpg" alt="Project screenshot 1">
          <img src="/assets/images/Placeholder.jpg" alt="Project screenshot 2">
          <img src="/assets/images/Placeholder.jpg" alt="Project screenshot 3">
          <img src="/assets/images/Placeholder.jpg" alt="Project screenshot 4">
        </div>
      </div>
    </section>

    <section class="section two-column-text">
      <div>
        <div class="orange-line"></div>
        <h2>Development Process</h2>
        <p>
          Use this section to explain how the project was made. You could talk about
          planning, prototyping, testing, feedback, and the changes you made during
          development.
        </p>
      </div>

      <div>
        <div class="orange-line"></div>
        <h2>My Role</h2>
        <p>
          Explain what parts of the project you created. This could include coding,
          design, artwork, animation, UI, sound, testing, or documentation.
        </p>
      </div>
    </section>

    <section class="section image-text-row">
      <img src="/assets/images/Placeholder.jpg" alt="Gameplay screenshot">

      <div>
        <div class="orange-line"></div>
        <h2>Main System</h2>
        <p>
          This is a good place to explain one of the most important parts of the
          project, such as the gameplay loop, combat system, level design, interaction
          system, or another major feature.
        </p>
      </div>
    </section>

    <section class="big-orange-section">
      <div class="orange-line" style="background: white;"></div>
      <h2>Reflection</h2>
      <p>
        Use this section to talk about what you learned from the project, what
        challenges you faced, and what you would improve if you continued working
        on it.
      </p>
    </section>

  </main>

</div>
