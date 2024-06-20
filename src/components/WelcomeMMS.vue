<script setup lang="ts">
defineProps<{
  msg: string
  class: string
}>()
</script>

<template>
  <div class="presentation">
    <div class="paragraph">
      <h3>Bienvenue chez MISSILLAC MARINE SERVICE 👋</h3>
      <p>
        Faites confiance à MISSILLAC MARINE SERVICE pour prendre soin de votre embarcation comme si
        c'était la nôtre.
      </p>
      <p>
        Explorez nos services et contactez-nous pour discuter de la meilleure manière de répondre à
        vos besoins maritimes uniques.
      </p>
      <p>Nous sommes impatients de vous offrir une expérience maritime exceptionnelle !</p>
      <div class="btn-container">
        <router-link id="btn-contact" class="contact-link" to="/contact">
          <h4>CONTACTEZ-NOUS</h4>
        </router-link>
        <router-link id="btn-services" class="services-link" to="/service">
          <h4>NOS SERVICES</h4>
        </router-link>
      </div>
    </div>
    <img class="img1" src="/images/sail_boat.jpg" alt="Image de bateau à voile" />
  </div>
</template>

<style scoped>
.presentation {
  margin: 2em;
  display: flex;
  background-color: #e7ecef;
}

.paragraph {
  flex: 1;
  text-align: justify;
  padding: 1em;
}

h3 {
  color: #274c77;
  font-size: 25px;
}

.btn-container {
  display: flex;
  justify-content: space-between;
  margin: 1em;
}

#btn-contact,
#btn-services {
  text-decoration: none;
  padding: 0 10px;
  white-space: nowrap;
  text-align: center;
  width: 50%;
  transition: all 0.5s ease;
}

#btn-contact:hover,
#btn-services:hover {
  background-color: rgb(158, 38, 38);
  color: white;
}

.contact-link {
  background-color: #a3cef1;
  color: #274c77;
  margin-right: 0.5em;
}

.services-link {
  background-color: #274c77;
  color: #a3cef1;
  margin-left: 0.5em;
}

.img1 {
  width: 50%;
  height: 25em;
  object-fit: cover;
}

@media (max-width: 1060px) {
  .img1 {
    display: none;
  }
}

@media (max-width: 450px) {
  .btn-container {
    flex-direction: column;
    margin: auto;
  }
  .contact-link,
  .services-link {
    margin: auto;
    margin-bottom: 1em;
    width: 100%;
  }
}
</style>
