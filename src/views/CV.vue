<template>
  <div class="cv">
    <div class="container">
      <h1>Curriculum Vitae</h1>
      <div class="cv-content">
        <section class="personal-info">
          <h2>Personal Information</h2>
          <p><strong>Name:</strong> Professor XXX</p>
          <p><strong>Title:</strong> Professor of Computer Science</p>
          <p><strong>Email:</strong> xxx@university.edu</p>
          <p><strong>Office:</strong> Building X, Room XXX</p>
        </section>
        <section class="education">
          <h2>Education</h2>
          <ul>
            <li>
              <h3>Ph.D. in Computer Science</h3>
              <p>University of XYZ, 20XX</p>
            </li>
            <li>
              <h3>M.S. in Computer Science</h3>
              <p>University of ABC, 20XX</p>
            </li>
            <li>
              <h3>B.S. in Computer Science</h3>
              <p>University of DEF, 20XX</p>
            </li>
          </ul>
        </section>
        <section class="experience">
          <h2>Professional Experience</h2>
          <ul>
            <li>
              <h3>Professor</h3>
              <p>University of XXX, 20XX - Present</p>
            </li>
            <li>
              <h3>Associate Professor</h3>
              <p>University of XXX, 20XX - 20XX</p>
            </li>
            <li>
              <h3>Assistant Professor</h3>
              <p>University of XXX, 20XX - 20XX</p>
            </li>
          </ul>
        </section>
        <section class="awards">
          <h2>Awards and Honors</h2>
          <ul>
            <li>Best Paper Award, International Conference on Machine Learning, 2023</li>
            <li>NSF CAREER Award, 2020</li>
            <li>Outstanding Teaching Award, University of XXX, 2019</li>
          </ul>
        </section>
      </div>
    </div>
  </div>
</template>

<script setup>
// CV page logic
</script>

<style scoped>
/* CV Page Styles */
.cv {
  padding: 4rem 0;
  font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
}

.container {
  max-width: 1200px;
  margin: 0 auto;
  padding: 0 1.5rem;
}

.cv h1 {
  font-size: 2.5rem;
  margin-bottom: 3rem;
  text-align: center;
  color: #1a237e;
  position: relative;
}

.cv h1::after {
  content: '';
  display: block;
  width: 80px;
  height: 3px;
  background-color: #2196f3;
  margin: 1rem auto 0;
}

.cv-content {
  display: grid;
  grid-template-columns: repeat(auto-fit, minmax(320px, 1fr));
  gap: 2.5rem;
}

section {
  background-color: #f9f9f9;
  padding: 2rem;
  border-radius: 12px;
  box-shadow: 0 3px 12px rgba(0, 0, 0, 0.05);
  transition: all 0.3s ease;
  border-left: 4px solid #2196f3;
}

section:hover {
  transform: translateY(-5px);
  box-shadow: 0 5px 15px rgba(0, 0, 0, 0.1);
}

section h2 {
  font-size: 1.6rem;
  margin-bottom: 1.5rem;
  color: #1a237e;
  border-bottom: 2px solid #2196f3;
  padding-bottom: 0.8rem;
  font-weight: 600;
}

ul {
  list-style: none;
  padding: 0;
}

li {
  margin-bottom: 1.5rem;
  position: relative;
  padding-left: 1.5rem;
}

li::before {
  content: '•';
  position: absolute;
  left: 0;
  top: 0.3rem;
  color: #2196f3;
  font-size: 1.2em;
  font-weight: bold;
}

li h3 {
  font-size: 1.2rem;
  margin-bottom: 0.5rem;
  color: #1a237e;
  font-weight: 600;
}

li p {
  margin: 0.5rem 0;
  color: #666;
  line-height: 1.6;
}

.personal-info p {
  margin: 0.8rem 0;
  color: #666;
  line-height: 1.6;
}

.personal-info strong {
  color: #1a237e;
  font-weight: 600;
}

/* Responsive Design */
@media (max-width: 992px) {
  .cv-content {
    grid-template-columns: 1fr;
  }
  
  section {
    padding: 1.8rem;
  }
}

@media (max-width: 768px) {
  .cv {
    padding: 3rem 0;
  }
  
  .cv h1 {
    font-size: 2rem;
  }
  
  section {
    padding: 1.5rem;
  }
  
  section h2 {
    font-size: 1.4rem;
  }
  
  li h3 {
    font-size: 1.1rem;
  }
}

@media (max-width: 480px) {
  .cv h1 {
    font-size: 1.8rem;
  }
  
  section {
    padding: 1.2rem;
  }
  
  section h2 {
    font-size: 1.3rem;
  }
  
  li {
    padding-left: 1.2rem;
  }
  
  li h3 {
    font-size: 1.05rem;
  }
}
</style>