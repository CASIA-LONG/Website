<template>
  <div class="team">
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
</template>

<script setup>
import teamData from '../data/team.json'
</script>

<style scoped>
.team {
  padding: 2rem 0;
  max-width: 1200px;
  margin: 0 auto;
  padding-left: 1rem;
  padding-right: 1rem;
}

h1 {
  font-size: 2.5rem;
  margin-bottom: 2rem;
  text-align: center;
}

.team-section {
  margin-bottom: 3rem;
  padding: 1.5rem;
  background-color: #f9f9f9;
  border-radius: 8px;
  box-shadow: 0 2px 4px rgba(0, 0, 0, 0.1);
}

.team-section h2 {
  font-size: 1.8rem;
  margin-bottom: 1.5rem;
  color: #333;
  border-bottom: 1px solid #ddd;
  padding-bottom: 0.5rem;
}

.member-grid {
  display: grid;
  grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
  gap: 2rem;
}

.member-card {
  text-align: center;
  padding: 1.5rem;
  background-color: #fff;
  border-radius: 8px;
  box-shadow: 0 1px 3px rgba(0, 0, 0, 0.05);
}

.member-photo {
  margin-bottom: 1rem;
}

.member-photo img {
  width: 150px;
  height: 150px;
  border-radius: 50%;
  object-fit: cover;
}

.member-card h3 {
  font-size: 1.2rem;
  margin-bottom: 0.5rem;
  color: #333;
}

.member-position {
  font-weight: 500;
  margin-bottom: 0.5rem;
  color: #555;
}

.member-email {
  margin-bottom: 1rem;
  color: #666;
}

.member-description {
  margin-bottom: 1.5rem;
  color: #666;
  line-height: 1.5;
}

.member-links {
  display: flex;
  justify-content: center;
  gap: 1rem;
  flex-wrap: wrap;
}

.link {
  color: #0066cc;
  text-decoration: none;
  font-size: 0.9rem;
  transition: color 0.3s ease;
}

.link:hover {
  color: #004080;
  text-decoration: underline;
}
</style>