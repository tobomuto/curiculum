<template>
  <div id="app">
    <div id="first">
      <BgFirst/>
      <Navbar/>
      <HelloWorld/>
    </div>
    <div id="second">      
      <About/>
    </div>
    <div id="third">      
      <Experiences/>
    </div>
    <div id="fourth">      
      <Contact/>
    </div>

  </div>
  
</template>

<script>

import BgFirst from './components/BgFirst.vue'
import Navbar from './components/Navbar.vue'
import HelloWorld from './components/HelloWorld.vue'
import About from './components/About.vue'
import Experiences from './components/Experiences.vue'
import Contact from './components/Contact.vue'

export default {
  name: 'App',
  components: {
    BgFirst,
    Navbar,
    HelloWorld,
    About,
    Experiences,
    Contact
  }
}
</script>

<style>

html {
  scroll-behavior: smooth;
}

#app {
  font-family: 'Lato', sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  color: rgb(236, 236, 236);
}


#first {
  height: 100vh;
  width: 100%;
  /* background-image: url("./assets/first.jpg"); */
  /* background: linear-gradient(to bottom, rgba(255,255,255,0.15) 0%, rgba(0,0,0,0.15) 100%), radial-gradient(at top center, rgba(255,255,255,0.40) 0%, rgba(0,0,0,0.40) 120%) #989898;
 background-blend-mode: multiply,multiply; */
}

#second{
  height: 100%;
  background: rgb(23,25,26);
  /* background: linear-gradient(320deg, rgba(23,25,26,1) 74%, rgba(33,36,37,1) 100%); */
}

#third{

  background: rgb(23,25,26);
}

#fourth{
  height: 100vh;
  background: rgb(23,25,26);
}


a {
    text-decoration: none;
    color: darkgrey;
}

a:hover {
    color: #344a42;
    text-decoration: none;
}


</style>
