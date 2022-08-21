<template>
  <v-container class="my-15">
    <v-row justify="center">
      <v-col lg="12" class="text-center">
        <v-subheader class="text-h4 justify-center">Portfolio </v-subheader>
        <p>
          Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do
          eiusmod
        </p>
      </v-col>
      <v-col lg="12">
        <div class="text-center">
          <v-chip
            @click="activePortfolio = 'webApp'"
            :color="activePortfolio === 'webApp' ? 'success' : ''"
            class="mx-5"
            >Web App</v-chip
          >
          <v-chip
            @click="activePortfolio = 'mobileApp'"
            :color="activePortfolio === 'mobileApp' ? 'success' : ''"
            class="mx-5"
            >Mobile App</v-chip
          >
          <v-chip
            @click="activePortfolio = 'desktopApp'"
            :color="activePortfolio === 'desktopApp' ? 'success' : ''"
            class="mx-5"
            >Desktop App</v-chip
          >
        </div>
      </v-col>
      <v-slot v-if="activePortfolio === 'mobileApp'">
        <v-col class="lg-3" v-for="(web, webindex) in webApps" :key="webindex">
          <v-card>
            <v-img
              src="card.src"
              class="white--text align-end"
              gradient="to bottom, rgba(0,0,0,.1),rgba(0,0,0,.5)"
              height="200px"
            >
              <v-card-title>
                {{ web.title }}
              </v-card-title>
            </v-img>
          </v-card>
        </v-col>
      </v-slot>
      <v-slot v-if="activePortfolio === 'mobileApp'">
        <v-col
          class="lg-3"
          v-for="(mobile, mobileindex) in mobileApps"
          :key="mobileindex"
        >
          <v-card>
            <v-img
              src="card.src"
              class="white--text align-end"
              gradient="to bottom, rgba(0,0,0,.1),rgba(0,0,0,.5)"
              height="200px"
            >
              <v-card-title>
                {{ mobile.title }}
              </v-card-title>
            </v-img>
          </v-card>
        </v-col>
      </v-slot>
      <v-slot v-if="activePortfolio === 'desktopApp'">
        <v-col
          class="lg-3"
          v-for="(desktop, desktopindex) in desktopApps"
          :key="desktopindex"
        >
          <v-card>
            <v-img
              src="card.src"
              class="white--text align-end"
              gradient="to bottom, rgba(0,0,0,.1),rgba(0,0,0,.5)"
              height="200px"
            >
              <v-card-title>
                {{ desktop.title }}
              </v-card-title>
            </v-img>
          </v-card>
        </v-col>
      </v-slot>
    </v-row>
  </v-container>
</template>

<script>
export default {
  name: "Portfolio",
  data() {
    return {
      activePortfolio: "webApp",
      webApps: [
        { title: "Web app1", image: "../assest/dev.jpeg" },
        { title: "Web app1", image: "../assest/dev.jpeg" },
        { title: "Web app1", image: "../assest/dev.jpeg" },
        { title: "Web app1", image: "../assest/dev.jpeg" },
        { title: "Web app1", image: "../assest/dev.jpeg" },
        { title: "Web app1", image: "../assest/dev.jpeg" },
        { title: "Web app1", image: "../assest/dev.jpeg" },
        { title: "Web app1", image: "../assest/dev.jpeg" },
        { title: "Web app1", image: "../assest/dev.jpeg" },
        { title: "Web app1", image: "../assest/dev.jpeg" },
      ],
      mobileApps: [
        { title: "Mobile app", image: "../assest/dev.jpeg" },
        { title: "Mobile app", image: "../assest/dev.jpeg" },
        { title: "Mobile app", image: "../assest/dev.jpeg" },
        { title: "Mobile app", image: "../assest/dev.jpeg" },
        { title: "Mobile app", image: "../assest/dev.jpeg" },
        { title: "Mobile app", image: "../assest/dev.jpeg" },
        { title: "Mobile app", image: "../assest/dev.jpeg" },
        { title: "Mobile app", image: "../assest/dev.jpeg" },
        { title: "Mobile app", image: "../assest/dev.jpeg" },
        { title: "Mobile app", image: "../assest/dev.jpeg" },
      ],
      desktopApps: [
        { title: "Desktop app", image: "../assest/dev.jpeg" },
        { title: "Desktop app", image: "../assest/dev.jpeg" },
        { title: "Desktop app", image: "../assest/dev.jpeg" },
        { title: "Desktop app", image: "../assest/dev.jpeg" },
        { title: "Desktop app", image: "../assest/dev.jpeg" },
        { title: "Desktop app", image: "../assest/dev.jpeg" },
        { title: "Desktop app", image: "../assest/dev.jpeg" },
        { title: "Desktop app", image: "../assest/dev.jpeg" },
        { title: "Desktop app", image: "../assest/dev.jpeg" },
        { title: "Desktop app", image: "../assest/dev.jpeg" },
      ],
    };
  },
};
</script>

<style></style>
