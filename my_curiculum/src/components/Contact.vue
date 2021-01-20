<template>

<div class="contact">

<b-container>

  

  <b-row>
    <b-col>
      <h3 class="sectionTitle">
          Me contacter
      </h3>
    </b-col>
  </b-row>

    
    <!-- <a href=""><img src="..\assets\icones\github-square.svg" alt="lien-github"></a>
    <a href=""><img src="..\assets\icones\linkedin.svg" alt="lien-linkedin"></a>
    <a href=""><img src="..\assets\icones\mail.svg" alt="lien-email"></a> -->
<b-row class="text-center">
  <b-col>
          <a href="https://www.linkedin.com/in/tombvr/" target="_blank"><i class="fab fa-linkedin-in fa-3x"></i></a>
  </b-col>
  <b-col>
          <a href="https://github.com/tobomuto" target="_blank"><i class="fab fa-github fa-3x"></i></a>
  </b-col>
  <b-col>
          <a href="mailto:tombvr75@gmail.com" target="_blank"><i class="fab far fa-envelope fa-3x"></i></a>
  </b-col>
</b-row>
  
</b-container>
</div>
</template>

<script>


export default {
    name: 'Contact',

}
</script>

<style scoped>

.contact {
  display: flex;
  align-items: center;
  height: 100%;
  padding: 3%;
}

.sectionTitle {
  text-transform: uppercase;
  color: #344a42;
  width: 100%;
  text-align: center;
}

.text-center {
  padding: 100px 0;
}
</style>