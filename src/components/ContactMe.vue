<template>
  <v-container class="my-15">
    <v-row justify="center">
      <v-col lg="12" class="text-center">
        <v-subheader class="text-h4 justify-center">Contact me </v-subheader>
        <p>
          Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do
          eiusmod
        </p>
      </v-col>
      <v-col lg="6">
        <iframe
          src="https://www.google.com/maps/embed?pb=!1m18!1m12!1m3!1d31526.713115929928!2d38.71328156924604!3d8.986945687195732!2m3!1f0!2f0!3f0!3m2!1i1024!2i768!4f13.1!3m3!1m2!1s0x164b869a8b536055%3A0x153e64699102a723!2sMekanisa%2C%20Addis%20Ababa!5e0!3m2!1sen!2set!4v1661102974959!5m2!1sen!2set"
          width="100%"
          height="100%"
          style="border: 0;"
          allowfullscreen=""
          loading="lazy"
          referrerpolicy="no-referrer-when-downgrade"
        ></iframe>
      </v-col>
      <v-col lg="6">
        <v-form ref="form" v-model="valid" lazy-validation>
          <v-text-field
            v-model="contactInfo.name"
            :counter="10"
            :rules="nameRules"
            label="Name"
            required
          >
          </v-text-field>
          <v-text-field
            v-model="contactInfo.email"
            :rules="emailRules"
            label="Email"
            required
          >
          </v-text-field>
          <v-text-area label="Message" v-model="contactInfo.message">
          </v-text-area>
          <v-btn color="success" class="mr-4">
            Send
          </v-btn>
        </v-form>
      </v-col>
    </v-row>
  </v-container>
</template>

<script>
export default {
  data() {
    return {
      contactInfo: [],
    };
  },
};
</script>

<style></style>
