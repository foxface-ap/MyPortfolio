<template>
  <Nav/>
  <Navbar/>
  <Projects/>
</template>

<script>
import Nav from './components/Nav.vue'
import Navbar from './components/Navbar.vue'
import Projects from './components/Projects.vue'

export default {
  name: 'App',
  components: {
    Nav,
    Navbar,
    Projects
  }
}
</script>

<style>

@import url('https://fonts.googleapis.com/css2?family=Mulish:wght@300;400&display=swap');


*{
  margin:0;
  box-sizing: border-box;
  font-family: 'Mulish', sans-serif;
}

body{
  background-color: #001b24;
  margin: 0;
  padding: 0;
}
.container{
  border-radius: 15px;
  position: relative;
  max-width: 1400px;
  width: 80%;
  min-height: 80%;
  height: 70%;
}

@media (max-width:767px)
{
  .container{
    border-radius: 15px;
    position: relative;
    max-width: 1400px;
    width: 90%;
    min-height: 80%;
    height: 70%;
  }
}
</style>
