<template>
  <div>

    <Header/>
    <HeroSection/>
    <AboutMe/>
    
    
  </div>
</template>

<script>
import Header from './components/HeaDer.vue'
import HeroSection from './components/HeroSection.vue'
import AboutMe from './components/About.vue'

export default{
  components:{
    Header,
    HeroSection,
    AboutMe,
  }
}
</script>

<style>
/* Add your styles here if needed */
</style>
