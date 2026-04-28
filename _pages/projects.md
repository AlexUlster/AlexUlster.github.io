---
title: "Projects"
layout: single
permalink: /projects/
sidebar:
  title: "Projects"
  nav:
    - projects
---

<style>
  /* Hero Section */
  .projects-hero {
    position: relative;
    height: 60vh;
    display: flex;
    align-items: center;
    justify-content: center;
    background: linear-gradient(135deg, #667eea 0%, #764ba2 100%);
    color: white;
    text-align: center;
    overflow: hidden;
    margin: -2rem -2rem 3rem -2rem;
  }

  .projects-hero::before {
    content: '';
    position: absolute;
    top: -50%;
    left: -50%;
    width: 200%;
    height: 200%;
    background: 
      radial-gradient(circle at 20% 50%, rgba(255,255,255,0.1) 0%, transparent 50%),
      radial-gradient(circle at 80% 80%, rgba(255,255,255,0.05) 0%, transparent 50%);
    animation: float 20s ease-in-out infinite;
  }

  @keyframes float {
    0%, 100% { transform: translate(0, 0) rotate(0deg); }
    50% { transform: translate(30px, -30px) rotate(180deg); }
  }

  .projects-hero-content {
    position: relative;
    z-index: 2;
    animation: fadeInUp 1s ease-out;
  }

  .projects-hero h1 {
    font-size: 3.5rem;
    margin-bottom: 1rem;
    font-weight: 700;
    text-shadow: 2px 2px 4px rgba(0,0,0,0.2);
  }

  .projects-hero p {
    font-size: 1.3rem;
    opacity: 0.95;
    max-width: 600px;
    margin: 0 auto;
  }

  /* Project Grid */
  .projects-container {
    display: grid;
    grid-template-columns: repeat(auto-fit, minmax(320px, 1fr));
    gap: 2rem;
    margin: 3rem 0;
  }

  .project-card {
    background: white;
    border-radius: 12px;
    overflow: hidden;
    box-shadow: 0 4px 6px rgba(0,0,0,0.1);
    transition: all 0.3s ease;
    cursor: pointer;
    animation: fadeInUp 0.6s ease-out backwards;
  }

  .project-card:nth-child(1) { animation-delay: 0.1s; }
  .project-card:nth-child(2) { animation-delay: 0.2s; }
  .project-card:nth-child(3) { animation-delay: 0.3s; }
  .project-card:nth-child(n+4) { animation-delay: 0.4s; }

  .project-card:hover {
    transform: translateY(-10px);
    box-shadow: 0 12px 24px rgba(0,0,0,0.15);
  }

  .project-image-container {
    position: relative;
    overflow: hidden;
    height: 250px;
    background: linear-gradient(135deg, #667eea 0%, #764ba2 100%);
  }

  .project-card img {
    width: 100%;
    height: 100%;
    object-fit: cover;
    transition: transform 0.3s ease;
  }

  .project-card:hover img {
    transform: scale(1.05);
  }

  .project-overlay {
    position: absolute;
    top: 0;
    left: 0;
    right: 0;
    bottom: 0;
    background: rgba(102, 126, 234, 0.9);
    display: flex;
    align-items: center;
    justify-content: center;
    opacity: 0;
    transition: opacity 0.3s ease;
  }

  .project-card:hover .project-overlay {
    opacity: 1;
  }

  .overlay-text {
    color: white;
    text-align: center;
    font-size: 1.1rem;
    font-weight: 600;
  }

  .project-content {
    padding: 1.5rem;
  }

  .project-title {
    font-size: 1.4rem;
    font-weight: 700;
    margin-bottom: 0.5rem;
    color: #333;
  }

  .project-description {
    color: #666;
    font-size: 0.95rem;
    margin-bottom: 1rem;
    line-height: 1.5;
  }

  .project-tags {
    display: flex;
    flex-wrap: wrap;
    gap: 0.5rem;
    margin-bottom: 1rem;
  }

  .project-tag {
    display: inline-block;
    background: linear-gradient(135deg, #667eea 0%, #764ba2 100%);
    color: white;
    padding: 0.3rem 0.8rem;
    border-radius: 20px;
    font-size: 0.8rem;
    font-weight: 600;
  }

  .project-link {
    display: inline-block;
    background: linear-gradient(135deg, #667eea 0%, #764ba2 100%);
    color: white;
    padding: 0.6rem 1.2rem;
    border-radius: 6px;
    text-decoration: none;
    font-weight: 600;
    transition: all 0.3s ease;
    border: none;
    cursor: pointer;
  }

  .project-link:hover {
    transform: translateX(5px);
    box-shadow: 0 4px 12px rgba(102, 126, 234, 0.4);
  }

  /* Scroll Indicator */
  .scroll-indicator {
    text-align: center;
    margin: 2rem 0;
    color: #999;
    font-size: 0.9rem;
  }

  .scroll-arrow {
    display: inline-block;
    animation: bounce 2s infinite;
  }

  @keyframes bounce {
    0%, 100% { transform: translateY(0); }
    50% { transform: translateY(-10px); }
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

  /* Responsive */
  @media (max-width: 768px) {
    .projects-hero h1 {
      font-size: 2rem;
    }

    .projects-hero p {
      font-size: 1rem;
    }

    .projects-container {
      grid-template-columns: 1fr;
      gap: 1.5rem;
    }
  }
</style>

<div class="projects-hero">
  <div class="projects-hero-content">
    <h1>My Projects</h1>
    <p>Exploring game design and development through creative projects</p>
  </div>
</div>

<div class="projects-container">
  <!-- Project 1 -->
  <div class="project-card">
    <div class="project-image-container">
      <img src="/assets/images/Placeholder.jpg" alt="Project 1">
      <div class="project-overlay">
        <div class="overlay-text">Click to explore →</div>
      </div>
    </div>
    <div class="project-content">
      <h3 class="project-title">Project 1</h3>
      <p class="project-description">A description of your first project goes here. Highlight the key features and what makes it unique.</p>
      <div class="project-tags">
        <span class="project-tag">Game Design</span>
        <span class="project-tag">Unity</span>
      </div>
      <a href="/projects/projects-pro1/" class="project-link">View Project</a>
    </div>
  </div>

  <!-- Project 2 -->
  <div class="project-card">
    <div class="project-image-container">
      <img src="/assets/images/Placeholder.jpg" alt="Project 2">
      <div class="project-overlay">
        <div class="overlay-text">Click to explore →</div>
      </div>
    </div>
    <div class="project-content">
      <h3 class="project-title">Project 2</h3>
      <p class="project-description">A description of your second project goes here. Showcase your skills and creative approach.</p>
      <div class="project-tags">
        <span class="project-tag">Development</span>
        <span class="project-tag">C#</span>
      </div>
      <a href="#" class="project-link">View Project</a>
    </div>
  </div>

  <!-- Project 3 -->
  <div class="project-card">
    <div class="project-image-container">
      <img src="/assets/images/Placeholder.jpg" alt="Project 3">
      <div class="project-overlay">
        <div class="overlay-text">Click to explore →</div>
      </div>
    </div>
    <div class="project-content">
      <h3 class="project-title">Project 3</h3>
      <p class="project-description">A description of your third project goes here. Tell the story of your development journey.</p>
      <div class="project-tags">
        <span class="project-tag">Narrative Design</span>
        <span class="project-tag">Unreal</span>
      </div>
      <a href="#" class="project-link">View Project</a>
    </div>
  </div>
</div>

<div class="scroll-indicator">
  <div class="scroll-arrow">↓ Scroll to see more ↓</div>
</div>

<script>
  // Scroll reveal animation
  const observerOptions = {
    threshold: 0.1,
    rootMargin: '0px 0px -100px 0px'
  };

  const observer = new IntersectionObserver((entries) => {
    entries.forEach(entry => {
      if (entry.isIntersecting) {
        entry.target.style.animation = 'fadeInUp 0.6s ease-out forwards';
        observer.unobserve(entry.target);
      }
    });
  }, observerOptions);

  document.querySelectorAll('.project-card').forEach(card => {
    observer.observe(card);
  });

  // Smooth scroll
  document.querySelectorAll('a[href^="#"]').forEach(anchor => {
    anchor.addEventListener('click', function (e) {
      e.preventDefault();
      const target = document.querySelector(this.getAttribute('href'));
      if (target) {
        target.scrollIntoView({
          behavior: 'smooth',
          block: 'start'
        });
      }
    });
  });
</script>
