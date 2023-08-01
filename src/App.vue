<template>
  <div class="container-fluid p-0">
    <HeaderTop />
    <HomeView />
    <!-- <nav>
      <router-link to="/">Home</router-link> |
      <router-link to="/about">About</router-link>
    </nav> -->
    <!-- <router-view /> -->
    <FooterSection />
  </div>
</template>
<script>
import HeaderTop from "./views/Navbar.vue";
import HomeView from "./views/HomeView.vue";
import FooterSection from "./views/Footer.vue";

export default {
  components: { HeaderTop, HomeView, FooterSection },
};
</script>

<style>
/* #app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
} */

nav {
  padding: 30px;
}

nav a {
  font-weight: bold;
  color: #2c3e50;
}

nav a.router-link-exact-active {
  color: #42b983;
}
</style>
