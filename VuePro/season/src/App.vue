<template>
  
  <Season/>
</template>

<script>
import Season from './components/Season.vue'

export default {
  name: 'App',
  components: {
    Season
  }
}
 
</script>

<style>
@import url('https://fonts.googleapis.com/css2?family=Satisfy&display=swap');
*{
    margin: 0;
padding: 0;
box-sizing: border-box;
font-family: 'Satisfy', cursive;
scroll-behavior: smooth;
}

body {
    overflow: hidden;
}


#app {
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
    width: 100%;
    height: 100vh;
    overflow: hidden;
} 
   
</style>
  



