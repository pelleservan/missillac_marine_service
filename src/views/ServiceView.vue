<script setup lang="ts">
import ServiceRange from '../components/ServiceRange.vue'
import Mobility from '../components/Mobility.vue'
import Transport from '../components/Transport.vue'
import TireService from '../components/TireService.vue'
</script>

<template>
  <main>
    <div class="container-head">
      <div class="head-container">
        <img class="head-img" src="/images/head.jpg" alt="boat image" />
        <div class="overlay"></div>
        <div class="sub-title">
          <h2>Acceuil >∏ Services</h2>
          <h1>CONTACT</h1>
        </div>
      </div>
    </div>
    <ServiceRange />
    <Mobility />
    <Transport />
    <TireService />
  </main>
</template>

<style scoped>
main {
  min-width: 300px;
}

.container-head {
  margin-top: 123px;
  position: relative;
  width: 100%;
  height: 50vh;
}

.sub-title {
  position: absolute;
  bottom: 0;
  color: white;
  z-index: 2;
  padding: 1em;
}

.sub-title h1 {
  font-size: 2em;
}

.sub-title h2 {
  font-size: 1em;
}

.head-container {
  position: relative;
  width: 100%;
  height: 100%;
  overflow: hidden;
  z-index: 1;
}

.head-img {
  position: absolute;
  top: 50%;
  left: 50%;
  width: 100%;
  height: 100%;
  object-fit: cover;
  transform: translate(-50%, -50%);
}

.overlay {
  position: absolute;
  top: 0;
  left: 0;
  width: 100%;
  height: 100%;
  background-color: rgba(0, 0, 0, 0.25);
  z-index: 1;
}
</style>
