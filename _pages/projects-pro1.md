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
  .project-page {
    max-width: 1000px;
    margin: 0 auto;
    padding: 1rem;
  }

  .project-section {
    margin-bottom: 3rem;
    animation: fadeInUp 0.7s ease-out;
  }

  .section-title {
    font-size: 2rem;
    color: #333;
    margin-bottom: 1rem;
  }

  .video-container {
    background: white;
    border-radius: 16px;
    padding: 1rem;
    box-shadow: 0 6px 18px rgba(0,0,0,0.12);
    border-top: 6px solid #f9b248;
  }

  .video-container iframe,
  .video-container video {
    width: 100%;
    aspect-ratio: 16 / 9;
    border: none;
    border-radius: 10px;
    display: block;
  }

  .info-card {
    background: white;
    border-radius: 16px;
    padding: 1.8rem;
    box-shadow: 0 4px 14px rgba(0,0,0,0.1);
    border-left: 6px solid #f9b248;
  }

  .info-card p {
    color: #666;
    line-height: 1.7;
    margin-bottom: 1rem;
  }

  .details-grid {
    display: grid;
    grid-template-columns: 1fr 1fr;
    gap: 1.5rem;
  }

  .detail-card {
    background: white;
    border-radius: 16px;
    padding: 1.5rem;
    box-shadow: 0 4px 14px rgba(0,0,0,0.1);
    border-top: 5px solid #f9b248;
  }

  .detail-card h3 {
    color: #333;
    margin-bottom: 0.7rem;
    font-size: 1.35rem;
  }

  .detail-card p {
    color: #666;
    line-height: 1.7;
  }

  .scrolling-gallery {
    overflow: hidden;
    border-radius: 16px;
    background: linear-gradient(135deg, #f9b248 0%, #f79e47 100%);
    box-shadow: 0 6px 18px rgba(0,0,0,0.12);
  }

  .gallery-track {
    display: flex;
    animation: scrollGallery 18s linear infinite;
  }

  .gallery-track:hover {
    animation-play-state: paused;
  }

  .gallery-track img {
    width: 320px;
    height: 210px;
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

  .large-image-section {
    display: grid;
    grid-template-columns: 1fr 1fr;
    gap: 2rem;
    align-items: center;
  }

  .large-image-section img {
    width: 100%;
    border-radius: 16px;
    box-shadow: 0 6px 18px rgba(0,0,0,0.14);
  }

  .large-image-text h3 {
    color: #333;
    font-size: 1.5rem;
    margin-bottom: 0.8rem;
  }

  .large-image-text p {
    color: #666;
    line-height: 1.7;
  }

  .highlight-box {
    background: linear-gradient(135deg, #f9b248 0%, #f79e47 100%);
    color: white;
    border-radius: 16px;
    padding: 2rem;
    box-shadow: 0 8px 24px rgba(249,178,72,0.35);
  }

  .highlight-box h2 {
    margin-bottom: 1rem;
    color: white;
  }

  .highlight-box p {
    line-height: 1.7;
    margin-bottom: 1rem;
  }

  @keyframes fadeInUp {
    from {
      opacity: 0;
      transform: translateY(25px);
    }
    to {
      opacity: 1;
      transform: translateY(0);
    }
  }

  @media (max-width: 768px) {
    .details-grid,
    .large-image-section {
      grid-template-columns: 1fr;
    }

    .gallery-track img {
      width: 260px;
      height: 170px;
    }
  }
</style>

<div class="project-page">

  <section class="project-section">
    <h1 class="section-title">Project 1</h1>

    <div class="video-container">
      <!-- YouTube embed version -->
      <iframe 
        src="https://www.youtube.com/embed/YOUR_VIDEO_ID_HERE"
        title="Project 1 Video Demo"
        allowfullscreen>
      </iframe>

      <!-- 
      If you want to use a local video instead, delete the iframe above and use this:

      <video controls>
        <source src="/assets/videos/project1-demo.mp4" type="video/mp4">
        Your browser does not support the video tag.
      </video>
      -->
    </div>
  </section>

  <section class="project-section">
    <div class="info-card">
      <h2 class="section-title">Project Overview</h2>

      <p>
        This section should introduce the project and explain what it is. Talk about
        the main idea, the genre, and what the player or user is expected to do.
      </p>

      <p>
        You can also mention your role in the project, what tools you used, and the
        main systems or features you personally worked on.
      </p>
    </div>
  </section>

  <section class="project-section">
    <h2 class="section-title">Image Gallery</h2>

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

  <section class="project-section">
    <div class="details-grid">
      <div class="detail-card">
        <h3>Development Process</h3>
        <p>
          Use this section to explain how the project was made. You could talk about
          early planning, prototypes, design changes, and how the project improved
          over time.
        </p>
      </div>

      <div class="detail-card">
        <h3>My Role</h3>
        <p>
          Explain what parts of the project you created. This could include coding,
          design, artwork, animation, UI, sound, testing, or documentation.
        </p>
      </div>
    </div>
  </section>

  <section class="project-section">
    <div class="large-image-section">
      <img src="/assets/images/Placeholder.jpg" alt="Project screenshot">

      <div class="large-image-text">
        <h3>Gameplay / Main System</h3>
        <p>
          This is a good place to explain one of the most important parts of the
          project. For example, you could describe the main gameplay loop, combat
          system, level design, interaction system, or another major feature.
        </p>
      </div>
    </div>
  </section>

  <section class="project-section">
    <div class="highlight-box">
      <h2>Reflection</h2>

      <p>
        Use this section to talk about what you learned from the project, what
        challenges you faced, and what you would improve if you continued working
        on it.
      </p>

      <p>
        This is also a good place to explain why the project is important in your
        portfolio and what skills it demonstrates.
      </p>
    </div>
  </section>

</div>
