<template>
  <div>
    <Start/>
    <Projects/>
    <About/>
    <Contact/>
  </div>

</template>

<script>
import Start from './components/Start.vue'
import Projects from './components/Projects.vue'
import About from './components/About.vue'
import Contact from './components/Contact.vue'
import 'animate.css';

export default {
  name: 'App',
  components: {
    Start,
    Projects,
    About,
    Contact
  }
}
</script>

<style>
  *{
    margin: 0;
    padding: 0;
  }

  html{
    height: 100%;
  }
  #app {
    font-family: Karla, sans-serif;
    font-size: 1.3rem;
    color: #696969
  }
</style>
