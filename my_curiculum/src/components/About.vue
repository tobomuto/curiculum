<template>
  <div class="about">
    <b-container class="cardSpace">
      <b-row align-v="start">
        <b-col md="4" xs="10" class="text-center">
          <Portrait />
        </b-col>  

        <b-col md="8" xs="10">
          <div class="intro">
          <h3 class="sectionTitle">
            à propos
          </h3>
          <p>
          Je suis Thomas Bouvier, Front-end Developer Junior.
          </p>
          <p>
            Après 10ans en tant qu'infographiste en retouche photographique,
            j'ai décidé de me réorienter professionellement. Ayant toujours eu
            un intérêt pour les nouvelles technologies, j'ai décidé de sauter le
            pas en intégrant la Coding Academy by Epitech à Paris, qui valorise
            l'apprentissage en autonomie, et en octobre 2020, j'ai écrit mes premières
            lignes de code. J'ai pu ensuite rejoindre l'équipe d'Open Mind Neurotechnologies 
            en tant que stagiaire développeur Front-End et participer à des projets passionnants. 
          </p>
          <p>
            Je me sens maintenant prêt à intégrer une nouvelle équipe et à faire face<br> à de nouveaux défis !
          </p>
          <b-row>
            <b-col class="p-3 text-center" >
              <CV/>
            </b-col>
          </b-row>

          </div>
        </b-col>
      </b-row>

    </b-container>
    
  </div>
</template>

<script>
import Portrait from "./Portrait.vue";
import CV from './CV.vue'

export default {
  name: "About",
  components: {
    Portrait,
    CV
  },
};
</script>

<style scoped>
.sectionTitle {
  top: 40px;
  text-transform: capitalize;
  color: #344a42;
  text-align: left;
}

.cardSpace {
  border-top: #2b2b2b solid 2px;
  border-left: #2b2b2b solid 2px;
  border-radius: 25px;
  background: rgb(23,25,26);
  box-shadow: 10px 10px 13px #141414,
              inset 10px 10px 13px #141414,
              -7px -7px 10px #1d1d1d,
              inset -7px -7px 10px #1d1d1d;
  z-index: 2;
}

.about {
  display: flex;
  align-items: center;
  height: 100%;
  padding: 3%;
}

.intro {
  padding: 50px;
}
</style>
