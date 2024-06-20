<script setup lang="ts">
defineProps<{
  msg: string
}>()
</script>

<template>
  <footer class="footer">
    <div class="upper-container">
      <div class="contact">
        <h2>Contact</h2>
        <a href="tel:+33687839238">Tel : 06 87 83 92 38</a>
        <a href="mailto:contact@missillac-marine-service.com"
          >eMail : contact@missillac-marine-service.com</a
        >
        <a href="geo:48.862725,2.287592?q=47%20rue%20du%20Pont-Saillant,%2044780%20Missillac"
          >Adresse : 47 rue du Pont-Saillant, 44 780 Missillac</a
        >
      </div>
      <div class="hours">
        <h2>Horaires d'ouverture</h2>
        <div class="hours-details">
          <div class="days">
            <p>Lundi</p>
            <p>Mardi</p>
            <p>Mercredi</p>
            <p>Jeudi</p>
            <p>Vendredi</p>
            <p>Samedi</p>
            <p>Dimanche</p>
          </div>
          <div class="open-hours">
            <p>Fermé</p>
            <p>9h - 12h / 14h - 18h</p>
            <p>9h - 12h / 14h - 18h</p>
            <p>9h - 12h / 14h - 18h</p>
            <p>9h - 12h / 14h - 18h</p>
            <p>9h - 12h / 14h - 18h</p>
            <p>Fermé</p>
          </div>
        </div>
      </div>
      <div>
        <h2>Naviguer sur notre site</h2>
        <div class="navbar-nav">
          <router-link class="link" to="/">ACCEUIL</router-link>
          <router-link class="link" to="/purpose">SERVICES</router-link>
          <router-link class="link" to="/purpose">VENTE</router-link>
          <router-link class="link" id="tire" to="/purpose">PNEUS</router-link>
        </div>
      </div>
    </div>
    <hr />
    <di class="down-container">
      <p>
        © 2024 - Missillac Marine Service -
        <a href="https://pelle-servan.fr/">Designed by Servan PELLÉ</a>
      </p>
    </di>
  </footer>
</template>

<style scoped>
footer {
  background-color: #274c77;
  color: white;
  padding: 1em;
}

.upper-container {
  display: flex;
  justify-content: space-between;
}

.contact {
  display: flex;
  flex-direction: column;
}

.contact a {
  text-decoration: none;
  color: white;
  margin-bottom: 10px;
  transition: all 0.3s;
}

.contact a:hover {
  color: rgb(158, 38, 38);
}

.hours-details {
  display: flex;
  justify-content: space-between;
  color: white;
}

.open-hours {
  text-align: right;
}

.navbar-nav {
  display: flex;
  flex-direction: column;
}

.navbar-nav .link {
  text-decoration: none;
  color: white;
  margin-bottom: 10px;
  transition: all 0.3s;
}

.navbar-nav .link:hover {
  color: rgb(158, 38, 38);
}

.down-container {
  text-align: center;
}

.down-container p a {
  text-decoration: none;
  color: white;
  transition: all 0.3s;
}

.down-container p a:hover {
  color: rgb(158, 38, 38);
}

@media (max-width: 900px) {
  .upper-container {
    flex-direction: column;
    width: 80%;
    margin: auto;
  }
}
</style>
