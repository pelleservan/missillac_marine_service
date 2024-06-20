<script setup lang="ts">
defineProps<{
  msg: string
}>()
</script>

<template>
  <header>
    <nav class="navbar" :class="{ scrolled: isScrolled }">
      <router-link to="/">
        <div class="navbar-logo">
          <h1>Missillac Marine Service</h1>
        </div>
      </router-link>
      <div class="navbar-quick">
        <router-link to="/contact">CONTACT</router-link>
      </div>
      <div class="navbar-nav">
        <router-link to="/">ACCEUIL</router-link>
        <router-link to="/purpose">SERVICES</router-link>
        <router-link to="/purpose">VENTE</router-link>
        <router-link id="tire" to="/purpose">PNEUS</router-link>
      </div>
    </nav>
  </header>
</template>

<style scoped>
@font-face {
  font-family: 'forum-regular';
  src: url('../../public/fonts/Forum-Regular.ttf') format('truetype');
}

.navbar {
  top: 0;
  left: 0;
  right: 0;
  position: fixed;
  z-index: 10;
  font-family: 'forum-regular';
  font-weight: bold;
  color: #e7ecef;
}

.navbar-logo {
  background-color: #274c77;
  position: absolute;
  padding: 5px 30px;
  font-size: 2em;
  border-radius: 0 0 50px 0;
  transition:
    padding 0.3s,
    font-size 0.3s;
}

.navbar-logo h1 {
  color: #e7ecef;
}

.navbar.scrolled .navbar-logo {
  padding: 0px 30px;
  font-size: 30px;
  transition:
    padding 0.3s,
    font-size 0.3s;
}

.navbar-quick {
  background-color: #274c77;
  padding: 10px;
  text-align: right;
  padding-top: 15px;
  padding-bottom: 15px;
}

.navbar-quick a {
  text-decoration: none;
  margin: 20px;
  color: #e7ecef;
  font-size: 20px;
  transition: 0.3s;
}

.navbar-quick a:hover {
  border-bottom: 2px solid;
}

.navbar-nav {
  background-color: #a3cef1;
  padding: 10px;
  text-align: right;
  padding-top: 25px;
  padding-bottom: 25px;
}

.navbar-nav a {
  text-decoration: none;
  padding: 20px;
  color: #e7ecef;
  font-size: 20px;
  transition: 0.3s;
}

.navbar-nav a:hover {
  color: #274c77;
}

#tire {
  border-left: 2px solid #e7ecef;
}

@media only screen and (max-width: 1080px) {
  .navbar-nav {
    display: none;
    flex-direction: column;
    position: absolute;
    top: 70px;
    left: 0;
    right: 0;
    background-color: #a3cef1;
    text-align: right;
    padding: 10px;
    transition: 0.5s;
  }

  .navbar-nav a {
    padding: 10px;
  }

  .mobile-menu {
    cursor: pointer;
  }

  .bar {
    width: 25px;
    height: 3px;
    background-color: #e7ecef;
    margin: 6px 0;
    transition: 0.4s;
  }

  .navbar.scrolled .navbar-nav {
    top: 100px;
  }

  .show-nav {
    display: flex;
  }
}
</style>
