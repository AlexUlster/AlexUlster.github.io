---
title: "Project 1"
layout: default
permalink: /projects/projects-pro1/
---

<style>
  .project-page {
    max-width: 1100px;
    margin: 0 auto;
    padding: 1rem;
  }

  .back-button {
    display: inline-block;
    margin: 1rem 0 2rem 0;
    background: linear-gradient(135deg, #f9b248 0%, #f79e47 100%);
    color: white;
    padding: 0.7rem 1.3rem;
    border-radius: 8px;
    text-decoration: none;
    font-weight: 700;
    transition: all 0.3s ease;
  }

  .back-button:hover {
    transform: translateX(-5px);
    box-shadow: 0 4px 12px rgba(249, 178, 72, 0.4);
  }

  .project-hero {
    position: relative;
    min-height: 380px;
    border-radius: 18px;
    overflow: hidden;
    background: linear-gradient(135deg, #f9b248 0%, #f79e47 100%);
    color: white;
    display: flex;
    align-items: flex-end;
    padding: 2.5rem;
    margin-bottom: 3rem;
    box-shadow: 0 8px 24px rgba(0,0,0,0.15);
  }

  .project-hero::before {
    content: '';
    position: absolute;
    inset: 0;
    background:
      linear-gradient(to top, rgba(0,0,0,0.55), rgba(0,0,0,0.05)),
      url("/assets/images/Placeholder.jpg");
    background-size: cover;
    background-position: center;
    opacity: 0.9;
  }

  .project-hero-content {
    position: relative;
    z-index: 2;
    max-width: 700px;
  }

  .project-hero h1 {
    font-size: 3.2rem;
    margin-bottom: 0.7rem;
    text-shadow: 2px 2px 6px rgba(0,0,0,0.3);
  }

  .project-hero p {
    font-size: 1.15rem;
    line-height: 1.6;
    opacity: 0.95;
  }

  .project-tags {
    display: flex;
    flex-wrap: wrap;
    gap: 0.6rem;
    margin-top: 1.2rem;
  }

  .project-tag {
    background: rgba(255,255,255,0.2);
    color: white;
    padding: 0.4rem 0.9rem;
    border-radius: 20px;
    font-size: 0.85rem;
    font-weight: 700;
    backdrop-filter: blur(4px);
  }

  .section-title {
    font-size: 2rem;
    color: #333;
    margin-bottom: 1rem;
  }

  .project-section {
    margin-bottom: 3.5rem;
    animation: fadeInUp 0.7s ease-out;
  }

  .overview-grid {
    display: grid;
    grid-template-columns: 1.2fr 0.8fr;
    gap: 2rem;
    align-items: start;
  }

  .info-card {
    background: white;
    border-radius: 14px;
    padding: 1.7rem;
    box-shadow: 0 4px 12px rgba(0,0,0,0.1);
  }

  .info-card p {
    color: #666;
    line-height: 1.7;
    margin-bottom: 1rem;
  }

  .quick-info {
    background: linear-gradient(135deg, #f9b248 0%, #f79e47 100%);
    color: white;
    border-radius: 14px;
    padding: 1.7rem;
    box-shadow: 0 4px 12px rgba(249,178,72,0.3);
  }

  .quick-info h3 {
    margin-bottom: 1rem;
    font-size: 1.4rem;
  }

  .quick-info p {
    margin: 0.6rem 0;
    line-height: 1.5;
  }

  .scrolling-gallery {
    overflow: hidden;
    border-radius: 14px;
    background: linear-gradient(135deg, #f9b248 0%, #f79e47 100%);
    box-shadow: 0 4px 12px rgba(0,0,0,0.12);
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

  .feature-grid {
    display: grid;
    grid-template-columns: repeat(auto-fit, minmax(240px, 1fr));
    gap: 1.5rem;
  }

  .feature-card {
    background: white;
    border-radius: 14px;
    padding: 1.5rem;
    box-shadow: 0 4px 12px rgba(0,0,0,0.1);
    border-top: 5px solid #f9b248;
    transition: all 0.3s ease;
  }

  .feature-card:hover {
    transform: translateY(-8px);
    box-shadow: 0 10px 22px rgba(0,0,0,0.14);
  }

  .feature-card h3 {
    color: #333;
    margin-bottom: 0.7rem;
    font-size: 1.25rem;
  }

  .feature-card p {
    color: #666;
    line-height: 1.6;
    font-size: 0.95rem;
  }

  .showcase-row {
    display: grid;
    grid-template-columns: 1fr 1fr;
    gap: 2rem;
    align-items: center;
    margin-bottom: 2rem;
  }

  .showcase-row:nth-child(even) .showcase-image {
    order: 2;
  }

  .showcase-image img {
    width: 100%;
    border-radius: 14px;
    box-shadow: 0 4px 12px rgba(0,0,0,0.15);
  }

  .showcase-text h3 {
    color: #333;
    font-size: 1.5rem;
    margin-bottom: 0.8rem;
  }

  .showcase-text p {
    color: #666;
    line-height: 1.7;
  }

  .video-container {
    background: white;
    border-radius: 14px;
    padding: 1rem;
    box-shadow: 0 4px 12px rgba(0,0,0,0.12);
  }

  .video-container iframe,
  .video-container video {
    width: 100%;
    aspect-ratio: 16 / 9;
    border: none;
    border-radius: 10px;
    display: block;
  }

  .final-card {
    background: linear-gradient(135deg, #f9b248 0%, #f79e47 100%);
    color: white;
    border-radius: 16px;
    padding: 2rem;
    text-align: center;
    box-shadow: 0 8px 24px rgba(249,178,72,0.35);
  }

  .final-card h2 {
    margin-bottom: 1rem;
  }

  .final-card p {
    max-width: 700px;
    margin: 0 auto;
    line-height: 1.7;
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
    .project-hero {
      min-height: 300px;
      padding: 1.5rem;
    }

    .project-hero h1 {
      font-size: 2.2rem;
    }

    .overview-grid,
    .showcase-row {
      grid-template-columns: 1fr;
    }

    .showcase-row:nth-child(even) .showcase-image {
      order: 0;
    }

    .gallery-track img {
      width: 260px;
      height: 170px;
    }
  }
</style>

<div class="project-page">

  <a href="/projects/" class="back-button">← Back to Projects</a>

  <div class="project-hero">
    <div class="project-hero-content">
      <h1>Project 1</h1>
      <p>
        A short introduction to the project goes here. Explain what the project is,
        what you made, and why it is interesting.
      </p>

      <div class="project-tags">
        <span class="project-tag">Game Design</span>
        <span class="project-tag">Unity</span>
        <span class="project-tag">C#</span>
        <span class="project-tag">Level Design</span>
      </div>
    </div>
  </div>

  <section class="project-section">
    <div class="overview-grid">
      <div class="info-card">
        <h2 class="section-title">Project Overview</h2>
        <p>
          This section should explain the main idea of your project. Talk about the goal,
          the type of game or experience you created, and what the player does.
        </p>
        <p>
          You can also mention your role in the project, such as programming, art,
          design, animation, UI, sound, or level design.
        </p>
      </div>

      <div class="quick-info">
        <h3>Quick Info</h3>
        <p><strong>Engine:</strong> Unity</p>
        <p><strong>Language:</strong> C#</p>
        <p><strong>Genre:</strong> Action / Adventure</p>
        <p><strong>Platform:</strong> PC</p>
        <p><strong>Status:</strong> In Development</p>
      </div>
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
    <h2 class="section-title">Key Features</h2>

    <div class="feature-grid">
      <div class="feature-card">
        <h3>Core Gameplay</h3>
        <p>
          Explain the main gameplay system here. For example, movement, combat,
          puzzle solving, exploration, or progression.
        </p>
      </div>

      <div class="feature-card">
        <h3>Visual Style</h3>
        <p>
          Describe the look of the project. Mention the art direction, UI style,
          animation style, or atmosphere.
        </p>
      </div>

      <div class="feature-card">
        <h3>Technical Work</h3>
        <p>
          Talk about the systems you built, such as enemy AI, scene transitions,
          player controls, UI, saving, or camera work.
        </p>
      </div>

      <div class="feature-card">
        <h3>What I Learned</h3>
        <p>
          Explain what skills you improved while making the project and what
          challenges you solved.
        </p>
      </div>
    </div>
  </section>

  <section class="project-section">
    <h2 class="section-title">Project Showcase</h2>

    <div class="showcase-row">
      <div class="showcase-image">
        <img src="/assets/images/Placeholder.jpg" alt="Gameplay screenshot">
      </div>

      <div class="showcase-text">
        <h3>Gameplay and Mechanics</h3>
        <p>
          Use this space to explain one important part of your project. This could be
          the player controller, combat system, enemy behaviour, level layout, or the
          main gameplay loop.
        </p>
      </div>
    </div>

    <div class="showcase-row">
      <div class="showcase-image">
        <img src="/assets/images/Placeholder.jpg" alt="Development screenshot">
      </div>

      <div class="showcase-text">
        <h3>Design Process</h3>
        <p>
          Explain how the project developed over time. You can talk about planning,
          prototyping, testing, feedback, and improvements you made.
        </p>
      </div>
    </div>
  </section>

  <section class="project-section">
    <h2 class="section-title">Video Demo</h2>

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
    <div class="final-card">
      <h2>Final Thoughts</h2>
      <p>
        End the page with a short reflection. Mention what you are proud of,
        what you would improve in the future, and what this project shows about
        your skills.
      </p>
    </div>
  </section>

</div>
