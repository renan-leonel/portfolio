<template>
  <Start/>
  <Projects/>
</template>

<script>
import Start from './components/Start.vue'
import Projects from './components/Projects.vue'
import 'animate.css';

export default {
  name: 'App',
  components: {
    Start,
    Projects
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
