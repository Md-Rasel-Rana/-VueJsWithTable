<template>
    <footer class="main-footer">
      <div class="footer-content">
        <div class="footer-logo">
          <!-- <img src="logo.png" alt="Logo"> -->
        </div>
        <div class="footer-links">
          <router-link to="/">Home</router-link>
          <router-link to="/about">About</router-link>
          <router-link to="/services">Services</router-link>
          <!-- Add more navigation links as needed -->
        </div>
      </div>
      <div class="footer-info">
        <p>&copy; 2024 Your Company. All rights reserved.</p>
      </div>
    </footer>
  </template>
  
  <script>
  export default {
    name: 'FooTer',
  };
  </script>
  
  <style scoped>
  /* Add your custom styles for the footer here */
  .main-footer {
    background-color: #333;
    color: #fff;
    padding: 1rem;
    text-align: center;
  }
  
  .footer-content {
    display: flex;
    justify-content: space-between;
    align-items: center;
  }
  
  .footer-logo img {
    max-height: 2.5rem;
  }
  
  .footer-links {
    display: flex;
  }
  
  router-link {
    color: #fff;
    text-decoration: none;
    margin-right: 1rem;
  }
  
  .footer-info {
    margin-top: 1rem;
  }
  
  /* Add more styles as needed */
  </style>
  