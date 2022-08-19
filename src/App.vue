<template>
  <v-app>
    <Header />
    <v-main>
      <HeroComponent />
    </v-main>
  </v-app>
</template>

<script>
import Header from "./components/Header.vue";
import HeroComponent from "./components/HeroComponent.vue";
export default {
  name: "App",

  components: { Header, HeroComponent },

  data: () => ({
    //
  }),
};
</script>
