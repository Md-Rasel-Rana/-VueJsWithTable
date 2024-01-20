<template>
    <div class="about-me-section">
      <div class="about-me-content">
        <h2>About Me</h2>
        <div class="profile-picture">
          <!-- <img src="profile-picture.jpg" alt="Profile Picture"> -->
        </div>
        <p>
          Hi, I'm [Your Name], a passionate web developer with a love for creating engaging and user-friendly applications using Vue.js.
        </p>
        <p>
          My journey in web development started [mention a brief background or timeline]. I specialize in front-end technologies, including HTML, CSS, and JavaScript. Vue.js has become my framework of choice for its simplicity and effectiveness in building dynamic and responsive user interfaces.
        </p>
        <p>
          I enjoy staying updated with the latest web development trends and technologies. When I'm not coding, you can find me exploring new libraries, contributing to open-source projects, or sharing my knowledge with the community.
        </p>
      </div>
    </div>
  </template>
  
  <script>
  export default {
    name: 'AboutMeSection',
  };
  </script>
  
  <style scoped>
  /* Add your custom styles for the about me section here */
  .about-me-section {
    background-color: #f5f5f5;
    padding: 4rem 0;
    text-align: center;
  }
  
  .about-me-content {
    max-width: 800px;
    margin: 0 auto;
  }
  
  .profile-picture img {
    border-radius: 50%;
    max-width: 100%;
    margin-bottom: 1.5rem;
  }
  
  h2 {
    font-size: 2.5rem;
    margin-bottom: 1.5rem;
  }
  
  p {
    font-size: 1.25rem;
    margin-bottom: 1.5rem;
  }
  
  /* Add more styles as needed */
  </style>
  