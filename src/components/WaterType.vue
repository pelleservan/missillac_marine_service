<script setup lang="ts">
defineProps<{
  msg: string
}>()
</script>

<template>
  <div class="water-container">
    <div class="half-container">
      <img class="half-img" src="/images/boat.jpg" />
      <div class="half-text">
        <h3>Eau salée</h3>
        <p>
          Des spécialistes de la mer. Votre bateau, préparé pour affronter les défis des eaux
          salées.
        </p>
        <router-link class="learn-link" to="/purpose">
          <h4>En savoir plus</h4>
        </router-link>
      </div>
    </div>
    <div class="half-container">
      <img class="half-img" src="/images/boot.jpg" />
      <div class="half-text">
        <h3>Eau douce</h3>
        <p>
          Des experts en navigation douce. Votre bateau, toujours prêt à conquérir les rivières et
          les lacs.
        </p>
        <router-link class="learn-link" to="/purpose">
          <h4>En savoir plus</h4>
        </router-link>
      </div>
    </div>
  </div>
</template>

<style scoped>
.water-container {
  display: flex;
  color: white;
}

.half-container {
  position: relative;
  width: 50%;
  overflow: hidden;
}

.half-container img {
  transition: all 0.5s;
}

.half-container:hover img {
  transform: scale(1.2);
}

.half-img {
  width: 100%;
  display: block;
}

.half-text {
  position: absolute;
  top: 0;
  left: 0;
  width: 100%;
  height: 100%;
  display: flex;
  flex-direction: column;
  justify-content: center;
  align-items: center;
  text-align: center;
  padding: 20px;
  background-color: rgba(0, 0, 0, 0.3);
  box-sizing: border-box;
}

.half-text h3 {
  margin-bottom: 10px;
  font-size: 2em;
}

.half-text p {
  margin-bottom: 15px;
  font-size: 1em;
}

.learn-link {
  text-decoration: none;
  font-weight: bold;
  background-color: #274c77;
  color: white;
  padding: 0 10px;
  transition: all 0.5s;
}

.learn-link:hover {
  background-color: rgb(158, 38, 38);
}

@media (max-width: 1060px) {
  .water-container {
    flex-direction: column;
  }
  .half-container {
    width: 100%;
  }
}
</style>
