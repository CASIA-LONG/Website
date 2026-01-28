<template>
  <div class="home">
    <!-- Hero Section -->
    <section class="hero">
      <div class="hero-content">
        <h1>RobotiXX Lab</h1>
        <p>Advanced Robotics Research at the Intersection of Motion Planning and Machine Learning</p>
      </div>
    </section>
    
    <!-- Group Profile Section -->
    <section class="group-profile">
      <div class="container">
        <h2>About the Group</h2>
        <div class="group-content">
          <div class="group-image">
            <div class="image-card">
              <img src="/group-profile.jpg" />
            </div>
          </div>
          <div class="group-about">
            <p class="mission-statement">
              At RobotiXX lab, researchers (XX-Men) and robots (XX-Bots) perform robotics research at the intersection of motion planning and machine learning with a specific focus on robustly deployable field robotics.
            </p>
            <p>
              Our research goal is to develop highly capable and intelligent mobile robots that are robustly deployable in the real world with minimal human supervision. XX-Men have vast experience deploying XX-Bots to tackle real-world problems in the field, building advanced robot platforms, developing complex sensing and actuation systems, designing sophisticated motion planning algorithms, and setting up standardized testbeds and metrics.
            </p>
            <p>
              We create highly capable and intelligent robots to locomote on land, in air, and at sea, pushing the boundaries of what's possible in robotics research.
            </p>
          </div>
        </div>
      </div>
    </section>
    
    <!-- Research Areas Section -->
    <section class="research-areas">
      <div class="container">
        <h2>Research Areas</h2>
        <div class="research-grid">
          <div class="research-card">
            <div class="research-icon">🤖</div>
            <h3>Robotics</h3>
            <p>Advanced robot platforms and systems</p>
          </div>
          <div class="research-card">
            <div class="research-icon">🧠</div>
            <h3>Machine Learning</h3>
            <p>Intelligent algorithms for robotics</p>
          </div>
          <div class="research-card">
            <div class="research-icon">📍</div>
            <h3>Motion Planning</h3>
            <p>Sophisticated path planning algorithms</p>
          </div>
          <div class="research-card">
            <div class="research-icon">🌍</div>
            <h3>Field Robotics</h3>
            <p>Robustly deployable real-world solutions</p>
          </div>
        </div>
      </div>
    </section>
    
    <!-- News and In Press Section -->
    <div class="container">
      <div class="news-inpress">
        <section class="news">
          <h2>News</h2>
          <ul class="news-list">
            <li class="news-item">
              <span class="news-date">Jan 2026</span>
              <span class="news-content">New research paper accepted</span>
            </li>
            <li class="news-item">
              <span class="news-date">Dec 2025</span>
              <span class="news-content">Lab receives new funding</span>
            </li>
            <li class="news-item">
              <span class="news-date">Nov 2025</span>
              <span class="news-content">New team member joins</span>
            </li>
            <li class="news-item">
              <span class="news-date">Oct 2025</span>
              <span class="news-content">Robot demonstration at conference</span>
            </li>
            <li class="news-item">
              <span class="news-date">Sep 2025</span>
              <span class="news-content">New robot platform developed</span>
            </li>
          </ul>
        </section>
        
        <section class="in-press">
          <h2>In Press</h2>
          <ul class="inpress-list">
            <li class="inpress-item">
              <span class="inpress-journal">Journal of Robotics Research</span>
              <span class="inpress-content">Novel motion planning algorithm</span>
            </li>
            <li class="inpress-item">
              <span class="inpress-journal">IEEE Transactions on Robotics</span>
              <span class="inpress-content">Field robotics deployment</span>
            </li>
            <li class="inpress-item">
              <span class="inpress-journal">Robotics and Autonomous Systems</span>
              <span class="inpress-content">Machine learning for robotics</span>
            </li>
            <li class="inpress-item">
              <span class="inpress-journal">International Journal of Robotics Research</span>
              <span class="inpress-content">Multi-robot coordination</span>
            </li>
            <li class="inpress-item">
              <span class="inpress-journal">Autonomous Robots</span>
              <span class="inpress-content">Robust navigation systems</span>
            </li>
          </ul>
        </section>
      </div>
    </div>
  </div>
</template>

<script setup>
// Home page logic
</script>

<style scoped>
/* Global Styles */
.home {
  font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
}

.container {
  max-width: 1200px;
  margin: 0 auto;
  padding: 0 1.5rem;
}

/* Hero Section */
.hero {
  background: linear-gradient(135deg, #1a237e 0%, #283593 100%);
  color: white;
  padding: 6rem 0;
  text-align: center;
  position: relative;
  overflow: hidden;
}

.hero::before {
  content: '';
  position: absolute;
  top: 0;
  left: 0;
  right: 0;
  bottom: 0;
  background: url('data:image/svg+xml;utf8,<svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 100 100" preserveAspectRatio="none"><path fill="rgba(255,255,255,0.05)" d="M0,0 L100,0 L100,100 Z"/></svg>');
  background-size: cover;
}

.hero-content {
  position: relative;
  z-index: 1;
}

.hero h1 {
  font-size: 3.5rem;
  margin-bottom: 1rem;
  font-weight: 700;
  letter-spacing: -0.5px;
}

.hero p {
  font-size: 1.3rem;
  max-width: 800px;
  margin: 0 auto;
  opacity: 0.9;
  line-height: 1.5;
}

/* Group Profile Section */
.group-profile {
  padding: 5rem 0;
  background-color: #f9f9f9;
}

.group-profile h2 {
  font-size: 2.2rem;
  margin-bottom: 3rem;
  text-align: center;
  color: #1a237e;
  position: relative;
}

.group-profile h2::after {
  content: '';
  display: block;
  width: 80px;
  height: 3px;
  background-color: #2196f3;
  margin: 1rem auto 0;
}

.group-content {
  display: flex;
  gap: 3rem;
  align-items: center;
}

.group-image {
  flex: 1;
  max-width: 550px;
}

.image-card {
  background-color: white;
  border-radius: 12px;
  overflow: hidden;
  box-shadow: 0 10px 30px rgba(0, 0, 0, 0.1);
  transition: transform 0.3s ease;
}

.image-card:hover {
  transform: translateY(-5px);
}

.image-card img {
  width: 100%;
  height: auto;
  display: block;
}

.group-about {
  flex: 1;
}

.mission-statement {
  font-size: 1.1rem;
  font-weight: 500;
  color: #333;
  margin-bottom: 1.5rem;
  line-height: 1.6;
}

.group-about p {
  color: #555;
  line-height: 1.7;
  margin-bottom: 1.2rem;
  font-size: 1rem;
}

/* Research Areas Section */
.research-areas {
  padding: 5rem 0;
  background-color: white;
}

.research-areas h2 {
  font-size: 2.2rem;
  margin-bottom: 3rem;
  text-align: center;
  color: #1a237e;
  position: relative;
}

.research-areas h2::after {
  content: '';
  display: block;
  width: 80px;
  height: 3px;
  background-color: #2196f3;
  margin: 1rem auto 0;
}

.research-grid {
  display: grid;
  grid-template-columns: repeat(auto-fit, minmax(280px, 1fr));
  gap: 2rem;
}

.research-card {
  background-color: #f9f9f9;
  padding: 2.5rem 2rem;
  border-radius: 12px;
  text-align: center;
  box-shadow: 0 5px 15px rgba(0, 0, 0, 0.05);
  transition: all 0.3s ease;
  border: 1px solid #eaeaea;
}

.research-card:hover {
  transform: translateY(-5px);
  box-shadow: 0 10px 25px rgba(0, 0, 0, 0.1);
  background-color: #f5f5f5;
}

.research-icon {
  font-size: 3rem;
  margin-bottom: 1.5rem;
  display: block;
}

.research-card h3 {
  font-size: 1.4rem;
  margin-bottom: 1rem;
  color: #1a237e;
  font-weight: 600;
}

.research-card p {
  color: #666;
  line-height: 1.5;
  font-size: 0.95rem;
}

/* News and In Press Section */
.news-inpress {
  display: grid;
  grid-template-columns: 1fr 1fr;
  gap: 3rem;
  padding: 4rem 0;
}

.news h2,
.in-press h2 {
  font-size: 1.8rem;
  margin-bottom: 2rem;
  color: #1a237e;
  text-align: left;
  position: relative;
}

.news h2::after,
.in-press h2::after {
  content: '';
  display: block;
  width: 60px;
  height: 2px;
  background-color: #2196f3;
  margin: 0.8rem 0 0;
}

.news-list,
.inpress-list {
  list-style: none;
  padding: 0;
}

.news-item,
.inpress-item {
  padding: 1rem 0;
  border-bottom: 1px solid #f0f0f0;
  transition: background-color 0.2s ease;
}

.news-item:hover,
.inpress-item:hover {
  background-color: #f9f9f9;
}

.news-date {
  display: block;
  font-size: 0.85rem;
  color: #999;
  font-weight: 500;
  margin-bottom: 0.3rem;
}

.news-content {
  display: block;
  color: #333;
  font-weight: 500;
}

.inpress-journal {
  display: block;
  font-size: 0.85rem;
  color: #2196f3;
  font-weight: 500;
  margin-bottom: 0.3rem;
}

.inpress-content {
  display: block;
  color: #333;
  font-weight: 500;
}

/* Responsive Design */
@media (max-width: 992px) {
  .hero h1 {
    font-size: 2.8rem;
  }
  
  .hero p {
    font-size: 1.1rem;
  }
  
  .group-content {
    flex-direction: column;
    text-align: center;
  }
  
  .group-image {
    max-width: 100%;
  }
  
  .news-inpress {
    grid-template-columns: 1fr;
    gap: 4rem;
  }
}

@media (max-width: 768px) {
  .hero h1 {
    font-size: 2.2rem;
  }
  
  .hero p {
    font-size: 1rem;
  }
  
  .group-profile h2,
  .research-areas h2 {
    font-size: 1.8rem;
  }
  
  .research-grid {
    grid-template-columns: 1fr;
  }
  
  .news h2,
  .in-press h2 {
    font-size: 1.5rem;
  }
}

@media (max-width: 480px) {
  .hero {
    padding: 4rem 0;
  }
  
  .hero h1 {
    font-size: 1.8rem;
  }
  
  .group-profile,
  .research-areas {
    padding: 3rem 0;
  }
  
  .group-content {
    gap: 2rem;
  }
  
  .research-card {
    padding: 2rem 1.5rem;
  }
}
</style>