<template>
  <v-container class="my-15">
    <v-row justify="center">
      <v-col lg="12" class="text-center">
        <v-subheader class="text-h4 justify-center">Project </v-subheader>
        <p>
          Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do
          eiusmod
        </p>
      </v-col>
      <v-col lg="4" v-for="project in 3" :key="project">
        <v-card class="mx-auto my-12" max-width="374">
          <v-img height="250" src="../assets/dev.jpeg"> </v-img>

          <v-card-title>
            Web Development
          </v-card-title>
          <v-card-text>
            <div>
              small plates, salads and sandwitches - an intimate setting with 12
              indoor sears pllsadj
            </div>
          </v-card-text>
          <v-divider class="mx-4"></v-divider>
          <v-card-actions>
            <v-btn color="success">View Details</v-btn>
            <v-spacer />
            <v-rating
              :value="4.5"
              color="amber"
              dense
              half-increments
              readonly
              size="14"
            ></v-rating>
          </v-card-actions>
        </v-card>
      </v-col> </v-row
  ></v-container>
</template>

<script>
export default {};
</script>

<style></style>
