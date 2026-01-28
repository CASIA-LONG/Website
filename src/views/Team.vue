<template>
  <div class="team">
    <div class="container">
      <h1>Our Team</h1>
      
      <!-- Faculty Section -->
      <section class="team-section">
        <h2>Faculty</h2>
        <div class="member-grid">
          <div v-for="(member, index) in teamData.faculty" :key="index" class="member-card">
            <div class="member-photo">
              <img :src="member.photo" :alt="member.name">
            </div>
            <h3>{{ member.name }}</h3>
            <p class="member-position">{{ member.position }}</p>
            <p class="member-email">{{ member.email }}</p>
            <p class="member-description">{{ member.description }}</p>
            <div class="member-links">
              <a v-if="member.links.website" :href="member.links.website" class="link" target="_blank">Website</a>
              <a v-if="member.links.google_scholar" :href="member.links.google_scholar" class="link" target="_blank">Google Scholar</a>
              <a v-if="member.links.github" :href="member.links.github" class="link" target="_blank">GitHub</a>
              <a v-if="member.links.linkedin" :href="member.links.linkedin" class="link" target="_blank">LinkedIn</a>
            </div>
          </div>
        </div>
      </section>
      
      <!-- Researchers Section -->
      <section class="team-section">
        <h2>Researchers</h2>
        <div class="member-grid">
          <div v-for="(member, index) in teamData.researchers" :key="index" class="member-card">
            <div class="member-photo">
              <img :src="member.photo" :alt="member.name">
            </div>
            <h3>{{ member.name }}</h3>
            <p class="member-position">{{ member.position }}</p>
            <p class="member-email">{{ member.email }}</p>
            <p class="member-description">{{ member.description }}</p>
            <div class="member-links">
              <a v-if="member.links.website" :href="member.links.website" class="link" target="_blank">Website</a>
              <a v-if="member.links.google_scholar" :href="member.links.google_scholar" class="link" target="_blank">Google Scholar</a>
              <a v-if="member.links.github" :href="member.links.github" class="link" target="_blank">GitHub</a>
              <a v-if="member.links.linkedin" :href="member.links.linkedin" class="link" target="_blank">LinkedIn</a>
            </div>
          </div>
        </div>
      </section>
      
      <!-- PhD Students Section -->
      <section class="team-section">
        <h2>PhD Students</h2>
        <div class="member-grid">
          <div v-for="(member, index) in teamData.phd_students" :key="index" class="member-card">
            <div class="member-photo">
              <img :src="member.photo" :alt="member.name">
            </div>
            <h3>{{ member.name }}</h3>
            <p class="member-position">{{ member.position }}</p>
            <p class="member-email">{{ member.email }}</p>
            <p class="member-description">{{ member.description }}</p>
            <div class="member-links">
              <a v-if="member.links.website" :href="member.links.website" class="link" target="_blank">Website</a>
              <a v-if="member.links.google_scholar" :href="member.links.google_scholar" class="link" target="_blank">Google Scholar</a>
              <a v-if="member.links.github" :href="member.links.github" class="link" target="_blank">GitHub</a>
              <a v-if="member.links.linkedin" :href="member.links.linkedin" class="link" target="_blank">LinkedIn</a>
            </div>
          </div>
        </div>
      </section>
      
      <!-- Master Students Section -->
      <section class="team-section">
        <h2>Master Students</h2>
        <div class="member-grid">
          <div v-for="(member, index) in teamData.master_students" :key="index" class="member-card">
            <div class="member-photo">
              <img :src="member.photo" :alt="member.name">
            </div>
            <h3>{{ member.name }}</h3>
            <p class="member-position">{{ member.position }}</p>
            <p class="member-email">{{ member.email }}</p>
            <p class="member-description">{{ member.description }}</p>
            <div class="member-links">
              <a v-if="member.links.website" :href="member.links.website" class="link" target="_blank">Website</a>
              <a v-if="member.links.google_scholar" :href="member.links.google_scholar" class="link" target="_blank">Google Scholar</a>
              <a v-if="member.links.github" :href="member.links.github" class="link" target="_blank">GitHub</a>
              <a v-if="member.links.linkedin" :href="member.links.linkedin" class="link" target="_blank">LinkedIn</a>
            </div>
          </div>
        </div>
      </section>
      
      <!-- Undergraduate Students Section -->
      <section class="team-section">
        <h2>Undergraduate Students</h2>
        <div class="member-grid">
          <div v-for="(member, index) in teamData.undergraduate_students" :key="index" class="member-card">
            <div class="member-photo">
              <img :src="member.photo" :alt="member.name">
            </div>
            <h3>{{ member.name }}</h3>
            <p class="member-position">{{ member.position }}</p>
            <p class="member-email">{{ member.email }}</p>
            <p class="member-description">{{ member.description }}</p>
            <div class="member-links">
              <a v-if="member.links.website" :href="member.links.website" class="link" target="_blank">Website</a>
              <a v-if="member.links.google_scholar" :href="member.links.google_scholar" class="link" target="_blank">Google Scholar</a>
              <a v-if="member.links.github" :href="member.links.github" class="link" target="_blank">GitHub</a>
              <a v-if="member.links.linkedin" :href="member.links.linkedin" class="link" target="_blank">LinkedIn</a>
            </div>
          </div>
        </div>
      </section>
    </div>
  </div>
</template>

<script setup>
import teamData from '../data/team.json'
</script>

<style scoped>
/* Team Page Styles */
.team {
  padding: 4rem 0;
  font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
}

.container {
  max-width: 1200px;
  margin: 0 auto;
  padding: 0 1.5rem;
}

.team h1 {
  font-size: 2.5rem;
  margin-bottom: 3rem;
  text-align: center;
  color: #1a237e;
  position: relative;
}

.team h1::after {
  content: '';
  display: block;
  width: 80px;
  height: 3px;
  background-color: #2196f3;
  margin: 1rem auto 0;
}

.team-section {
  margin-bottom: 4rem;
  padding: 2rem;
  background-color: #f9f9f9;
  border-radius: 12px;
  box-shadow: 0 2px 8px rgba(0, 0, 0, 0.05);
  transition: all 0.3s ease;
}

.team-section:hover {
  box-shadow: 0 4px 16px rgba(0, 0, 0, 0.1);
}

.team-section h2 {
  font-size: 1.8rem;
  margin-bottom: 2rem;
  color: #1a237e;
  border-bottom: 2px solid #2196f3;
  padding-bottom: 0.8rem;
  font-weight: 600;
}

.member-grid {
  display: grid;
  grid-template-columns: repeat(auto-fit, minmax(320px, 1fr));
  gap: 2.5rem;
}

.member-card {
  text-align: center;
  padding: 2rem;
  background-color: #fff;
  border-radius: 12px;
  box-shadow: 0 3px 12px rgba(0, 0, 0, 0.08);
  transition: all 0.3s ease;
  border: 1px solid #eaeaea;
  position: relative;
  overflow: hidden;
}

.member-card::before {
  content: '';
  position: absolute;
  top: 0;
  left: 0;
  right: 0;
  height: 4px;
  background: linear-gradient(90deg, #2196f3, #1a237e);
}

.member-card:hover {
  transform: translateY(-8px);
  box-shadow: 0 8px 24px rgba(0, 0, 0, 0.12);
  border-color: #2196f3;
}

.member-photo {
  margin-bottom: 1.5rem;
  position: relative;
  display: inline-block;
}

.member-photo img {
  width: 160px;
  height: 160px;
  border-radius: 50%;
  object-fit: cover;
  border: 4px solid #f0f0f0;
  transition: all 0.3s ease;
}

.member-card:hover .member-photo img {
  border-color: #2196f3;
  transform: scale(1.05);
}

.member-card h3 {
  font-size: 1.3rem;
  margin-bottom: 0.8rem;
  color: #1a237e;
  font-weight: 600;
}

.member-position {
  font-weight: 500;
  margin-bottom: 0.8rem;
  color: #555;
  font-size: 0.95rem;
}

.member-email {
  margin-bottom: 1.2rem;
  color: #666;
  font-size: 0.9rem;
}

.member-description {
  margin-bottom: 1.8rem;
  color: #666;
  line-height: 1.6;
  font-size: 0.95rem;
}

.member-links {
  display: flex;
  justify-content: center;
  gap: 1.2rem;
  flex-wrap: wrap;
  padding-top: 1rem;
  border-top: 1px solid #f0f0f0;
}

.link {
  color: #2196f3;
  text-decoration: none;
  font-size: 0.9rem;
  transition: all 0.3s ease;
  font-weight: 500;
  position: relative;
}

.link::after {
  content: '';
  position: absolute;
  bottom: -2px;
  left: 0;
  width: 0;
  height: 1px;
  background-color: #2196f3;
  transition: width 0.3s ease;
}

.link:hover {
  color: #1a237e;
}

.link:hover::after {
  width: 100%;
}

/* Responsive Design */
@media (max-width: 992px) {
  .member-grid {
    grid-template-columns: repeat(auto-fit, minmax(280px, 1fr));
    gap: 2rem;
  }
  
  .member-card {
    padding: 1.8rem;
  }
}

@media (max-width: 768px) {
  .team {
    padding: 3rem 0;
  }
  
  .team h1 {
    font-size: 2rem;
  }
  
  .team-section {
    padding: 1.5rem;
    margin-bottom: 3rem;
  }
  
  .team-section h2 {
    font-size: 1.5rem;
  }
  
  .member-grid {
    grid-template-columns: 1fr;
  }
  
  .member-card {
    padding: 1.5rem;
  }
  
  .member-photo img {
    width: 140px;
    height: 140px;
  }
}

@media (max-width: 480px) {
  .team h1 {
    font-size: 1.8rem;
  }
  
  .team-section h2 {
    font-size: 1.3rem;
  }
  
  .member-card {
    padding: 1.2rem;
  }
  
  .member-links {
    gap: 1rem;
  }
}
</style>