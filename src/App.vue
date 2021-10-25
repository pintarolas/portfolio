<template>
  <div id="app">
    <navbar-component />
    <about-me />
    <project />
    <contact />
    <footer-component />
  </div>
</template>

<script>
import AboutMe from "./components/AboutMeComponent.vue";
import Project from "./components/ProjectComponent.vue";
import FooterComponent from "./components/FooterComponent.vue";
import Contact from "./components/ContactComponent.vue";
import NavbarComponent from "./components/NavbarComponent.vue";

export default {
  name: "App",
  components: {
    AboutMe,
    Project,
    Contact,
    FooterComponent,
    NavbarComponent,
  },
};
</script>

<style>
#app {
  font-family: Verdana, Geneva, Tahoma, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
}
</style>
