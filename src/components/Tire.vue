<script setup lang="ts">
defineProps<{
  msg: string
}>()
</script>

<template>
  <div class="tire-container">
    <img id="tire" src="/images/tire.jpg" alt="Tire Image" />
    <div class="content">
      <h2>Montage de pneumatiques</h2>
      <p>
        Chez Missillac Marine Service, nous allons au-delà des vagues avec notre service de montage
        de pneus automobiles.
      </p>
      <router-link class="tire-link" to="/purpose">
        <h4>En savoir plus</h4>
      </router-link>
      <p>
        Profitez d'un vaste réseau de partenaires pour découvrir et acheter vos pneus au meilleur
        prix.
      </p>
      <div class="partenaire-container">
        <a href="https://www.allopneus.com/" target="_blank">
          <img src="/images/allopneus.png" alt="Allopneus" />
        </a>
        <a href="https://www.1001pneus.fr/" target="_blank">
          <img src="/images/1001pneus.png" alt="1001pneus" />
        </a>
        <a href="https://www.centralepneus.fr/" target="_blank">
          <img src="/images/centralepneus.png" alt="Centralepneus" />
        </a>
        <a href="https://www.123pneus.fr/" target="_blank">
          <img src="/images/123pneus.png" alt="123pneus" />
        </a>
        <a href="https://www.pneus-online.fr//" target="_blank">
          <img src="/images/pneus_online.png" alt="123pneus" />
        </a>
      </div>
    </div>
  </div>
</template>

<style scoped>
.tire-container {
  display: flex;
  margin: 2em;
  background-color: #e7ecef;
  text-align: center;
}

h2 {
  font-size: 2em;
}

img {
  width: 30%;
}

.content {
  padding: 1em;
  text-align: center;
  color: #274c77;
}

.tire-link {
  text-decoration: none;
  width: auto;
  display: flex;
  text-align: center;
}

.tire-link h4 {
  background-color: #274c77;
  color: white;
  transition: all 0.5s;
  padding: 10px;
  margin: auto;
}

.tire-link h4:hover {
  background-color: rgb(158, 38, 38);
}

.partenaire-container {
  display: flex;
  justify-content: space-between;
  align-items: center;
}

.partenaire-container a {
  width: 19%;
  height: 100%;
  align-items: center;
  margin: auto;
  transition: all 0.3s;
  border: 2px solid rgba(158, 38, 38, 0);
  border-radius: 3px;
}

.partenaire-container img {
  width: 100%;
  margin: auto;
}

.partenaire-container a:hover {
  border-bottom: 2px solid rgb(158, 38, 38);
}

@media (max-width: 1060px) {
  #tire {
    display: none;
  }
  .content {
    width: 100%;
  }
}

@media (max-width: 650px) {
  .partenaire-container {
    flex-direction: column;
    width: 100%;
  }
  .partenaire-container a {
    width: 100%;
  }
}
</style>
