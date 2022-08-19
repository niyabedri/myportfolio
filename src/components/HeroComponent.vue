<template>
  <v-container class="mt-0 pt-0">
    <v-row>
      <v-col lg="6">
        <h2 class="intro-text">Welcome to my Portfolio</h2>
        <p class="description">
          Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do
          eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad
          minim veniam, quis nostrud exercitation ullamco laboris nisi ut
          aliquip ex ea commodo consequat.
        </p>
        <v-btn color="success" rounded>Explore about me</v-btn>
      </v-col>
      <v-col lg="6">
        <img width="100%" height="100%" src="../assets/Me.jpg" alt="" />
      </v-col>
    </v-row>
  </v-container>
</template>

<script>
export default {};
</script>

<style>
h2.intro-text {
  font-size: 60px;
  font-weight: bold;
  font-family: cursive;
  color: #444;
}

p.description {
}
</style>
