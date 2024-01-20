<template>
    <table class="table mt-5">
      <thead>
        <tr>
          <th scope="col">#</th>
          <th scope="col">First</th>
          <th scope="col">Last</th>
          <th scope="col">Phone</th>
          <th scope="col">Email</th>
          <th scope="col">Action</th>
        </tr>
      </thead>
      <tbody>
        <tr v-for="(data, index) in content" :key="index">
          <th scope="row">{{ index + 1 }}</th>
          <td>{{ data.firstName }}</td>
          <td>{{ data.lastName }}</td>
          <td>{{ data.phone }}</td>
          <td>{{ data.email }}</td>
          <td><button class="btn btn-danger btn-md" @click="DeleteRow(index)">Delete</button></td>
          <!-- Repeat this line for each data field -->
        </tr>
      </tbody>
    </table>
  </template>
  
  <script>
  export default {
    name: 'HeroSection',
    methods:{
      DeleteRow(index){
        this.content.splice(index,1);
      }
    },
    data() {
      return {
        content: [
          {
            firstName: 'John',
            lastName: 'Doe',
            phone: '01643599933',
            email: 'Johndoe@gmail.com'
          },
          {
            firstName: 'Alice',
            lastName: 'Smith',
            phone: '0123456789',
            email: 'alice.smith@example.com'
          },
          {
            firstName: 'Bob',
            lastName: 'Johnson',
            phone: '9876543210',
            email: 'bob.johnson@example.com'
          }
          // Add more data objects as needed
        ]
      };
    },
  };
  </script>
  
  
  <style scoped>
  /* Add your custom styles for the hero section here */
  .hero-section {
    background: url('hero-image.jpg') center/cover no-repeat;
    color: #000000;
    text-align: center;
    padding: 4rem 0;
  }
  
  .hero-content {
    max-width: 600px;
    margin: 0 auto;
  }
  
  h1 {
    font-size: 2.5rem;
    margin-bottom: 1rem;
  }
  
  p {
    font-size: 1.25rem;
    margin-bottom: 1.5rem;
  }
  
  .cta-button {
    display: inline-block;
    background-color: #3498db;
    color: #fff;
    padding: 0.75rem 1.5rem;
    text-decoration: none;
    border-radius: 5px;
    transition: background-color 0.3s;
  }
  
  .cta-button:hover {
    background-color: #2980b9;
  }
  
  /* Add more styles as needed */
  </style>
  