<template>
  <div class="chronologie">

      <h3 class="sectionTitle" id="chronologie">Chronologie</h3>

      <div class="ligne"></div>

      <div class="rond r1" data-anim="1"></div>
      <div class="rond r2" data-anim="2"></div>
      <div class="rond r3" data-anim="3"></div>
      <div class="rond r4" data-anim="4"></div>
      <div class="rond r5" data-anim="5"></div>

      <div class="box b1">
        <h6>2021</h6>
        <h4>Développeur Front End (Stage)</h4>
        <h5><a href="https://www.omind.me/">OPEN MIND NEUROTECHNOLOGIES</a>, (FULL-REMOTE)</h5>
        <ul>
          <li>-Intégration HTML5/CSS3(SASS/LESS) des maquettes adobeXD (VueJs)</li>
          <li>-Création puis maintenance du front-end du service web (VueJs)</li>
          <li>-Dialogue avec l'API via Axios et traitement des datas</li>
          <li>-Intégration des templates emailing via MJML</li>
          <li>-Pair-programming avec le développeur back-end</li>

        </ul>
      </div>

      <div class="box b2">
        <h6>2020-présent</h6>
        <h4>Formation développement web front-end</h4>
        <h5><a href="https://www.coding-academy.fr/">CODING ACADEMY BY EPITECH</a>, PARIS</h5>
        <ul>
          <li>-Bases de la programmation web, de ses langages et frameworks.</li>
          <li>-Maquettes UI et intégration responsive.</li>
        </ul>
      </div>

      <div class="box b3">
      <h6>2011-2019</h6>
      <h4>RETOUCHEUR PHOTO EXPERT</h4>
      <h5><a href="http://lacenstudio.com/">LACEN STUDIO</a>, PARIS</h5>
      <ul>
        <li>
          -Retouches digitales, compositing : Automobile, 3D, CGI, Beautés et
          Mode, Nature morte, Web & Print. Compositing, montages...
        </li>
        <li>-Développement photographies RAW sur CaptureOne.</li>
        <li>-Traitements colorimétriques vidéo sur After Effect.</li>
      </ul>
      </div>

      <div class="box b4">
      <h6>2008-2010</h6>
      <h4>MAQUETTISTE (ALTERNANCE)</h4>
      <h5>TALON HAUT STUDIO, PARIS</h5>
      <ul>
        <li>-Réalisation de maquettes pour le magazine Talon Haut Magazine.</li>
        <li>-Retouches et traitement colorimétriques des photographies.</li>
        <li>
          -Participation à la mise en oeuvre du Festival International de la
          photographie de mode à Cannes.
        </li>
      </ul>
      </div>
      
      <div class="box b5">
      <h6>2008-2010</h6>
      <h4>BAC PRO - ARTISANNAT ET MÉTIERS D’ART, OPTION COMMUNICATION GRAPHIQUE (ALTERNANCE)</h4>
      <h5>Campus Fonderie de l’Image, BAGNOLET</h5>
      </div>

      <!-- <div class="box b5">
      <h6>2006-2008</h6>
      <h4>CAP DESSINATEUR D’EXÉCUTION EN COMMUNICATION GRAPHIQUE</h4>
      <h5>Lycée Corvisart, Paris</h5>
      </div> -->

  </div>
</template>

<script>

import { gsap } from "gsap";
import { ScrollTrigger } from "gsap/ScrollTrigger";
gsap.registerPlugin(ScrollTrigger);

export default {
  name: "Experiences",
  mounted: 
  function(){
    this.scrollAnimation()
  },
  methods: {
   scrollAnimation: function() {
    gsap.from('.b1', {
      scrollTrigger: {
        trigger: '.r1',
        start: "top center",
      },
      x: -300,
      ease: "power3",
      opacity: 0, 
      duration: 1
    })
    gsap.from('.b2', {
      scrollTrigger: {
        trigger: '.r2',
        start: "top center",
      },
      x: 300,
      ease: "power3",
      opacity: 0, 
      duration: 1
    })
    gsap.from('.b3', {
      scrollTrigger: {
        trigger: '.r3',
        start: "top center",
      },
      x: -300,
      ease: "power3",
      opacity: 0, 
      duration: 1
    })
    gsap.from('.b4', {
      scrollTrigger: {
        trigger: '.r4',
        start: "top center",
      },
      x: 300,
      ease: "power3", 
      opacity: 0, 
      duration: 1
    })
    gsap.from('.b5', {
      scrollTrigger: {
        trigger: '.r5',
        start: "top center",
      },
      x: -300,
      ease: "power3",
      opacity: 0, 
      duration: 1
    })                
   }
 }
};
</script>

<style scoped>

.chronologie {
  width: 100%;
  height: 1600px;
  margin: 0 auto;
  padding: 80px 0 250px 0;
  position: relative;
}

.ligne {
    height: 1200px;
    width: 5px;
    margin: 100px auto;
    background: #344a42;
}

.rond {
    width: 30px;
    height: 30px;
    border-radius: 50%;
    border: #344a42 solid 2px;
    background: rgb(33, 36, 37);
    position: absolute;
    left: 50%;
    transform: translate(-50%);
    display: flex;
    justify-content: center;
    align-items: center;
    font-size: 40px;
    box-shadow: inset 5px 5px 8px #141414,
                -7px -7px 10px #1d1d1d;    
}

.r1{top: 215px;}
.r2{top: 515px;}
.r3{top: 805px;}
.r4{top: 1095px;}
.r5{top: 1270px;}

.box {
    width: 400px;
    min-height: 150px;
    padding: 20px;
    border-radius: 25px;
    height: auto;
    background: rgb(30, 33, 34);
    box-shadow: 10px 10px 13px #141414,
                -7px -7px 10px #1d1d1d;
    position: absolute;
    left: 50%;
    transform: translate(-50%);
    font-size: 0.8rem;
}

.b1 {
    top: 215px;
    left: calc(50% - 270px);
}
.b2 {
    top: 515px;
    left: calc(50% + 270px);
}
.b3 {
    top: 805px;
    left: calc(50% - 270px);
}
.b4 {
    top: 1095px;
    left: calc(50% + 270px);
}
.b5 {
    top: 1270px;
    left: calc(50% - 270px);
}

@media screen and (max-width: 1000px) {
  .ligne {
      position: relative;
      left: 180px;
  }
  .rond {
      left: calc(50% + 180px);
  }
  .box {
      width: 350px;
      left: calc(50% - 27px)
  }
}


.sectionTitle {
  top: 40px;
  text-transform: capitalize;
  color: #344a42;
  width: 100%;
  text-align: center;
  font-size: 2rem;
}

h1, h2, h3, h4, h5, h6 {
  text-transform: uppercase;
  font-size: 0.9rem;
}

h4 {
  font-weight: bold;
}

h6 {
  color: #344a42;
}

ul li {
  list-style: none;
}

</style>
