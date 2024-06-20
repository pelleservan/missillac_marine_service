<script setup lang="ts">
import WelcomeMMS from '../components/WelcomeMMS.vue'
import PartnerMMS from '../components/PartnerMMS.vue'
import WaterType from '../components/WaterType.vue'
import Tire from '../components/Tire.vue'
</script>

<template>
  <main>
    <div class="container-video">
      <div class="sub-title">
        <h1>TOUS MATÉRIELS NAUTIQUES</h1>
        <hr />
        <h2>VENTE - RÉPARATION - NÉGOCE - ENTRETIEN</h2>
      </div>
      <div class="video-container">
        <video autoplay loop muted>
          <source src="/videos/home.mp4" type="video/mp4" />
        </video>
        <img class="overlay-image" src="/images/video_cover.png" />
      </div>
    </div>
    <WelcomeMMS class="welcome-mms" />
    <PartnerMMS />
    <WaterType />
    <Tire />
  </main>
</template>

<style scoped>
@font-face {
  font-family: 'forum-regular';
  src: url('../../public/fonts/Forum-Regular.ttf') format('truetype');
}

body,
html {
  margin: 0;
  padding: 0;
  font-family: 'forum-regular';
  position: absolute;
}

main {
  min-width: 100%;
  margin: 0;
  padding: 0;
  left: 0;
  box-sizing: border-box;
}

.container-video {
  margin-top: 123px;
  position: relative;
  width: 100%;
  height: 50vh;
}

.sub-title {
  position: absolute;
  top: 0;
  width: auto;
  height: 100%;
  color: white;
  z-index: 2;
  padding: 1em;
  font-size: 2em;
  /* background: rgba(0, 0, 0, 0.2); */
}

.video-container {
  position: absolute;
  top: 0;
  width: 100%;
  height: 100%;
  overflow: hidden;
  z-index: 1;
}

video {
  position: absolute;
  top: 50%;
  left: 50%;
  width: 100%;
  height: 100%;
  object-fit: cover;
  transform: translate(-50%, -50%);
}

.overlay-image {
  position: absolute;
  bottom: 0;
  width: 100%;
  height: auto;
  opacity: 0.5;
  z-index: 3;
}

.welcome-mms {
  margin-top: 1em;
}

@media (max-width: 650px) {
  .sub-title {
    font-size: 1.5em;
  }
}
</style>
