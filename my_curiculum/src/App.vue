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
      <Studies/>
    </div>
    <div id="fifth">      
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
import Studies from './components/Studies.vue'
import Contact from './components/Contact.vue'

export default {
  name: 'App',
  components: {
    BgFirst,
    Navbar,
    HelloWorld,
    About,
    Experiences,
    Studies,
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
  color: #ffffff;
}

  /* text-align: center;
  color: #2c3e50;
  margin-top: 60px; */


#first {
  height: 100vh;
  width: 100%;
  /* background-image: url("./assets/first.jpg"); */
  /* background: linear-gradient(to bottom, rgba(255,255,255,0.15) 0%, rgba(0,0,0,0.15) 100%), radial-gradient(at top center, rgba(255,255,255,0.40) 0%, rgba(0,0,0,0.40) 120%) #989898;
 background-blend-mode: multiply,multiply; */
}

#second{
  height: 100vh;
  background: #1E1E1E;
}

#third{
  height: 100vh;
  background: #7a7a7a;
}

#fourth{
  height: 100vh;
  background: #272727;
}

#fifth{
  height: 100vh;
  background-image: url("./assets/contact.jpg");
}



a {
    text-decoration: none;
  
}

.sectionTitle {
  text-transform: capitalize;
}


</style>
