<template>
  <div class="open-hour">
    <img src="/public/images/dock.jpg" alt="dock image" style="width: 70%; height: auto" />

    <div class="content">
      <h2>HORAIRES D'OUVERTURE 🚪</h2>
      <p>
        Nous vous remercions pour votre confiance et votre intérêt pour MISSILLAC MARINE SERVICE.
        Nous avons hâte de collaborer avec vous et de vous aider à profiter pleinement de vos
        expériences nautiques.
      </p>
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
  </div>
</template>

<style scoped>
.open-hour {
  margin-top: 123px;
  display: flex;
  margin: 2em;
  background-color: #e7ecef;
  min-width: 300px;
}

.content {
  width: 50%;
  padding: 1em;
  text-align: justify;
}

h2 {
  color: #274c77;
}

.hours-details {
  display: flex;
  justify-content: space-between;
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
