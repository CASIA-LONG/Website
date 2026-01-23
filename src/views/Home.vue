<template>
  <div class="home">
    <section class="hero">
      <div class="hero-content">
        <h1>Welcome to XXX Lab</h1>
      </div>
    </section>
    <section class="group-profile">
      <div class="group-content">
        <div class="group-image">
          <img src="/group-profile.jpg" alt="Group Profile" />
        </div>
        <div class="group-about">
          <h2>About the Group</h2>
          <p>
            At RobotiXX lab, researchers (XX-Men) and robots (XX-Bots) perform robotics research at the intersection of motion planning and machine learning with a specific focus on robustly deployable field robotics. Our research goal is to develop highly capable and intelligent mobile robots that are robustly deployable in the real world with minimal human supervision. XX-Men have vast experience deploying XX-Bots to tackle real-world problems in the field, building advanced robot platforms, developing complex sensing and actuation systems, designing sophisticated motion planning algorithms, and setting up standardized testbeds and metrics in order to create highly capable and intelligent robots to locomote on land, in air, and at sea.
          </p>
        </div>
      </div>
    </section>
    <section class="news">
      <h2>News</h2>
      <ul>
        <li>abc</li>
        <li>abc</li>
        <li>abc</li>
        <li>abc</li>
        <li>abc</li>
        <li>abc</li>
        <li>abc</li>
        <li>abc</li>
      </ul>
    </section>
    <section class="in-press">
      <h2>In Press</h2>
      <ul>
        <li>abc</li>
        <li>abc</li>
        <li>abc</li>
        <li>abc</li>
        <li>abc</li>
        <li>abc</li>
        <li>abc</li>
        <li>abc</li>
      </ul>
    </section>
  </div>
</template>

<script setup>
// Home page logic
</script>

<style scoped>
.home {
  padding: 2rem 0;
}

.hero {
  background-color: #f5f5f5;
  padding: 4rem 0;
  text-align: center;
}

.hero-content h1 {
  font-size: 2.5rem;
  margin-bottom: 1rem;
}

.hero-content p {
  font-size: 1.2rem;
  color: #666;
}

.group-profile {
  padding: 3rem 0;
  max-width: 1200px;
  margin: 0 auto;
  padding-left: 1rem;
  padding-right: 1rem;
}

.group-content {
  display: flex;
  gap: 2rem;
  align-items: flex-start;
}

.group-image {
  flex: 1;
  max-width: 500px;
}

.group-image img {
  width: 100%;
  height: auto;
  border-radius: 8px;
  box-shadow: 0 2px 8px rgba(0, 0, 0, 0.1);
}

.group-about {
  flex: 1;
}

.news,
.in-press {
  padding: 3rem 0;
  max-width: 1200px;
  margin: 0 auto;
  padding-left: 1rem;
  padding-right: 1rem;
}

h2 {
  font-size: 2rem;
  margin-bottom: 1.5rem;
  text-align: center;
}

p {
  color: #333;
  line-height: 1.6;
}

@media (max-width: 768px) {
  .group-content {
    flex-direction: column;
  }
  
  .group-image {
    max-width: 100%;
  }
}
</style>