<template>
  <div class="hello">
    <b-container fluid>
    <h1 class="title">Thomas Bouvier</h1>
    <h2 class="subtitle">Junior Front-End Developer</h2>
    </b-container>
  </div>
</template>

<script>

import { gsap } from 'gsap';

export default {
  name: 'HelloWorld',
  mounted: function(){
    this.startAnimation()
  },
  methods: {
    startAnimation: function() {
    gsap.from('.title, .subtitle', {duration: 1.5, y: -30, opacity: 0, stagger: 0.7})
    }
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>

.hello {
  width: 100%;
  text-align: center;
  position: absolute;
  top: 40%;
}

.title {
  /* text-transform: uppercase; */
  font-size: 6rem;
  margin: 20 0px;
  font-family: 'Marcellus', serif;
  mix-blend-mode: difference;
}

.subtitle {
  font-family: 'Lato', sans-serif;
  margin: 10px;
  font-size: 1.5em;
  mix-blend-mode: difference;
}

</style>
