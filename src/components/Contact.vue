<script setup lang="ts">
defineProps<{
  msg: string
}>()
</script>

<template>
  <div class="contact">
    <div class="content">
      <h2>CONTACTEZ-NOUS 📞</h2>
      <p>
        Nous sommes à votre disposition pour répondre à toutes vos questions concernant nos services
        de vente, réparation, négoce et entretien de matériel nautique. Que vous soyez un passionné
        de nautisme ou un professionnel du secteur, notre équipe est là pour vous offrir des
        solutions sur mesure adaptées à vos besoins.
      </p>
      <div class="contact-link">
        <a href="tel:+33687839238">Tel : 06 87 83 92 38</a>
        <a href="mailto:contact@missillac-marine-service.com"
          >eMail : contact@missillac-marine-service.com</a
        >
        <a href="geo:48.862725,2.287592?q=47%20rue%20du%20Pont-Saillant,%2044780%20Missillac"
          >Adresse : 47 rue du Pont-Saillant, 44 780 Missillac</a
        >
      </div>
    </div>
    <img class="head-img" src="/public/images/contact.jpg" alt="boat image" />
  </div>
</template>

<style scoped>
.contact {
  margin-top: 123px;
  display: flex;
  margin: 2em;
  background-color: #e7ecef;
}

.content {
  width: 50%;
  padding: 1em;
  text-align: justify;
  min-width: 300px;
}

h2 {
  color: #274c77;
}

.contact-link {
  display: flex;
  flex-direction: column;
  font-size: 1.5em;
}

.contact-link a {
  text-decoration: none;
  color: #274c77;
  margin-bottom: 10px;
  transition: all 0.3s;
}

.contact-link a:hover {
  color: rgb(158, 38, 38);
}

img {
  width: 50%;
}

@media (max-width: 1100px) {
  img {
    display: none;
  }
  .content {
    width: 100%;
  }
}
</style>
