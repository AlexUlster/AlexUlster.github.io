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

  .info-card-container {
    display: grid;
    grid-template-columns: repeat(3, 1fr);
    gap: 2rem;
  }

  .info-card {
    background: white;
    border-radius: 12px;
    overflow: hidden;
    box-shadow: 0 4px 6px rgba(0,0,0,0.1);
    transition: all 0.3s ease;
    animation: fadeInUp 0.6s ease-out backwards;
  }

  .info-card:nth-child(1) { animation-delay: 0.1s; }
  .info-card:nth-child(2) { animation-delay: 0.2s; }
  .info-card:nth-child(3) { animation-delay: 0.3s; }

  .info-card:hover {
    transform: translateY(-10px);
    box-shadow: 0 12px 24px rgba(0,0,0,0.15);
  }

  .info-image-container {
    height: 220px;
    overflow: hidden;
    background: linear-gradient(135deg, #f7b147 0%, #f79e47 100%);
  }

  .info-image-container img {
    width: 100%;
    height: 100%;
    object-fit: cover;
    transition: transform 0.3s ease;
  }

  .info-card:hover img {
    transform: scale(1.05);
  }

  .info-content {
    padding: 1.5rem;
  }

  .info-title {
    font-size: 1.4rem;
    font-weight: 700;
    margin-bottom: 0.5rem;
    color: #333;
  }

  .info-description {
    color: #666;
    font-size: 0.95rem;
    line-height: 1.5;
    margin-bottom: 1rem;
  }

  .info-tags {
    display: flex;
    flex-wrap: wrap;
    gap: 0.5rem;
  }

  .info-tag {
    display: inline-block;
    background: linear-gradient(135deg, #f7b147 0%, #f79e47 100%);
    color: white;
    padding: 0.3rem 0.8rem;
    border-radius: 20px;
    font-size: 0.8rem;
    font-weight: 600;
  }

  @keyframes fadeInUp {
    from {
      opacity: 0;
      transform: translateY(30px);
    }
    to {
      opacity: 1;
      transform: translateY(0);
    }
  }

  @media (max-width: 768px) {
    .project-scale {
      width: 100%;
    }

    .project-video-scale {
      transform: none;
      width: 100%;
      margin-bottom: 2rem;
    }

    .info-card-container {
      grid-template-columns: 1fr;
      gap: 1.5rem;
    }
  }
</style>

<div class="project-scale">

  <h1 class="project-title">Project 1</h1>

  <div class="project-video-scale">
    <div class="video-container">
      <iframe 
        src="https://www.youtube.com/embed/YOUR_VIDEO_ID_HERE"
        title="Project Video"
        allowfullscreen>
      </iframe>
    </div>
  </div>

  <div class="info-card-container">

    <div class="info-card">
      <div class="info-image-container">
        <img src="/assets/images/Placeholder.jpg" alt="Project overview">
      </div>

      <div class="info-content">
        <h3 class="info-title">Overview</h3>
        <p class="info-description">
          Explain what the project is, the main goal, and what the player or user does.
        </p>

        <div class="info-tags">
          <span class="info-tag">Game Design</span>
          <span class="info-tag">Unity</span>
        </div>
      </div>
    </div>

    <div class="info-card">
      <div class="info-image-container">
        <img src="/assets/images/Placeholder.jpg" alt="Development process">
      </div>

      <div class="info-content">
        <h3 class="info-title">Development</h3>
        <p class="info-description">
          Talk about how the project was made, what changed during development, and what you improved.
        </p>

        <div class="info-tags">
          <span class="info-tag">Development</span>
          <span class="info-tag">C#</span>
        </div>
      </div>
    </div>

    <div class="info-card">
      <div class="info-image-container">
        <img src="/assets/images/Placeholder.jpg" alt="Main system">
      </div>

      <div class="info-content">
        <h3 class="info-title">Main System</h3>
        <p class="info-description">
          Break down an important system, such as combat, enemy AI, UI, mechanics, or level design.
        </p>

        <div class="info-tags">
          <span class="info-tag">Systems</span>
          <span class="info-tag">Gameplay</span>
        </div>
      </div>
    </div>

  </div>

</div>
