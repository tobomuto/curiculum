<template>
  <div class="hello">
    <b-container fluid>
    <h1 class="title">Thomas Bouvier</h1>
    <h2 class="subtitle">Junior Front-End Developer</h2>
    </b-container>
  </div>
</template>

<script>
export default {
  name: 'HelloWorld',
  props: {

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

/* hr {
  background-color: white;
  width: 6rem;
} */

.title {
  /* text-transform: uppercase; */
  font-size: 6rem;
  margin: 20 0px;
  font-family: 'Playfair Display', serif;

}

.subtitle {
  font-family: 'Lato', sans-serif;
  margin: 10px;
  font-size: 1.5em;
}

</style>
