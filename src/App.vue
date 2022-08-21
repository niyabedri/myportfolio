<template>
  <v-app>
    <Header />
    <v-main>
      <HeroComponent />
      <AboutMe />
      <Portfolio />
      <Project />
      <Gallery />
      <Contact />
      <Footer />
    </v-main>
  </v-app>
</template>

<script>
import Header from "./components/Header.vue";
import HeroComponent from "./components/HeroComponent.vue";
import AboutMe from "./components/AboutMe.vue";
import Portfolio from "./components/Portfolio.vue";
import Project from "./components/Project.vue";
import Gallery from "./components/Gallery.vue";
import Contact from "./components/ContactMe.vue";
import Footer from "./components/Footer.vue";
export default {
  name: "App",

  components: {
    Header,
    HeroComponent,
    AboutMe,
    Portfolio,
    Project,
    Gallery,
    Contact,
    Footer,
  },

  data: () => ({
    //
  }),
};
</script>
