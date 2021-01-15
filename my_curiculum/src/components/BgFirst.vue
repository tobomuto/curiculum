<template>
    

    <div class="backgroundBorder">
        <div class="background">

            <svg>
            <filter id="turbulence" x="0" y="0" width="100%" height="100%">
                <feTurbulence id="sea-filter" numOctaves="12" seed="6" baseFrequency="0.03 0.03"></feTurbulence>
                <feDisplacementMap scale="7" in="SourceGraphic"></feDisplacementMap>
                <animate xlink:href="#sea-filter" attributeName="baseFrequency" dur="120s" keyTimes="0;0.5;1" values="0.02 0.06;0.04 0.08;0.02 0.06" repeatCount="indefinite"/>
            </filter>
            </svg>
        </div>
      </div>
</template>

<script>
export default {
    name: 'BgFirst'

}
</script>

<style>

.backgroundBorder {
  position: absolute;
  top: 0vh;
  left: 0vh;
  height: 100vh;
  width: 100%;
  background-image: url("../assets/first.jpg");
}



.background {
  position: absolute;
  top: -0vh;
  left: 0vh;
  height: 100vh;
  width: 100%;
  background-image: url("../assets/first.jpg");
  background-size: cover;
  filter:url("#turbulence");

}

</style>