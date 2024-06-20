<script setup lang="ts">
defineProps<{
  msg: string
}>()
</script>

<template>
  <div class="activities-container">
    <h2>MISSILLAC MARINE SERVICE : Votre Partenaire Maritime de Confiance 👍🏻</h2>
    <div class="act-container">
      <div class="sub-pres">
        <div class="activity-title">
          <router-link class="link" to="/service">
            <h3>Gamme Complète de Services</h3>
            <img class="img" src="/images/engine.jpg" />
          </router-link>
        </div>
        <router-link class="middle-link" to="/service">
          <h4>Gamme Complète de Services</h4>
        </router-link>
        <p>
          Bienvenue chez MISSILLAC MARINE SERVICE, votre partenaire de confiance pour tous les
          besoins liés à votre embarcation. Notre chantier naval vous offre une gamme complète de
          services, allant de l'entretien mécanique (essence, diesel, hors-bord, in-bord...) à la
          transformation intérieure, en passant par l'électricité, l'électronique, la
          stratification, le traitement osmotique, la peinture, et bien plus encore.
        </p>
        <router-link class="little-link" to="/service">En savoir plus →</router-link>
      </div>
      <div class="sub-pres">
        <div class="activity-title">
          <router-link class="link" to="/service">
            <h3>Flexibilité avec Notre Chantier Mobile</h3>
            <img class="img" src="/images/driver.jpg" />
          </router-link>
        </div>
        <router-link class="middle-link" to="/service">
          <h4>Flexibilité avec Notre Chantier Mobile</h4>
        </router-link>
        <p>
          Dotés d'un chantier mobile, nous sommes flexibles et prêts à intervenir directement sur
          votre lieu d'amarrage si nécessaire. Chez MISSILLAC MARINE SERVICE, nous comprenons
          l'importance de maintenir votre embarcation en parfait état, et c'est pourquoi nous
          mettons à votre disposition notre expertise et notre dévouement.
        </p>
        <router-link class="little-link" to="/service">En savoir plus →</router-link>
      </div>
      <div class="sub-pres">
        <div class="activity-title">
          <router-link class="link" to="/service">
            <h3>Opérations de Manutention et Transport</h3>
            <img class="img" src="/images/manu.jpg" />
          </router-link>
        </div>
        <router-link class="middle-link" to="/service">
          <h4>Opérations de Manutention et Transport</h4>
        </router-link>
        <p>
          Au-delà des travaux techniques, nous sommes également spécialisés dans l'organisation des
          opérations de manutention de votre bateau et proposons des services de transport vers la
          destination de votre choix. Nous faisons de votre satisfaction notre priorité, et notre
          équipe expérimentée est prête à relever tous les défis pour assurer la sécurité et la
          performance de votre navire.
        </p>
        <router-link class="little-link" to="/service">En savoir plus →</router-link>
      </div>
    </div>
  </div>
</template>

<style scoped>
.activities-container {
  margin: 2em;
  background-color: #e7ecef;
  text-align: justify;
  padding: 1em;
}

h2 {
  color: #274c77;
  font-size: 25px;
}

.act-container {
  display: flex;
  justify-content: space-between;
}

.sub-pres {
  width: 30%;
  display: flex;
  flex-direction: column;
}

.activity-title {
  position: relative;
}

.activity-title h3 {
  position: absolute;
  top: 0;
  left: 0;
  bottom: +0.2em;
  width: 100%;
  height: auto;
  background-color: rgba(0, 0, 0, 0.5);
  color: white;
  padding: 0.5em;
  margin: 0;
  box-sizing: border-box;
  transition: all 0.5s;
}

.act-container h3:hover {
  background-color: rgba(158, 38, 38, 0.8);
}

.img {
  width: 100%;
  height: auto;
  max-width: 100%;
  object-fit: cover;
}

.middle-link {
  text-decoration: none;
  color: #274c77;
  font-size: 20px;
}

.link {
  text-decoration: none;
  color: white;
  text-align: center;
}

.little-link {
  color: #274c77;
  text-decoration: none;
}

.link:hover,
.middle-link:hover,
.little-link:hover {
  color: rgb(158, 38, 38);
}

@media (max-width: 1060px) {
  .act-container {
    flex-direction: column;
  }
  .sub-pres {
    width: 100%;
  }
  .activity-title {
    display: none;
  }
  .little-link {
    margin-bottom: 10px;
  }
  .sub-pres {
    border-bottom: 1px solid white;
  }
}
</style>
