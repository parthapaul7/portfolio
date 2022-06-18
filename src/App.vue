<template>
  <div>
    <Navbar/>
    <Home/>
  </div>
</template>

<script>
import Navbar from '@/components/navbar/Navbar.vue'
import Home from '@/components/home/Home.vue'

export default {
  name: 'App',
  components: {
    Navbar,
    Home
  }
}
</script>

<style>
@import url('https://fonts.googleapis.com/css2?family=Roboto+Mono&family=Roboto:wght@100&display=swap');

:root{
  --nav-blue:#21325E;
  --primary-dark:#1D1D1D;
  --primary-blue:#3E497A;
  --primary-yelllow:#F1D00A;
}
#app {
  margin: 0;
  padding: 0;
  border: 0;
}
body{
  margin: 0;
  font-family: 'Roboto Mono', monospace;
  background-color: var(--primary-dark);
}
</style>
