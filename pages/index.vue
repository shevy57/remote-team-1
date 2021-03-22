<template>
  <v-row justify="center" align="center">
    <v-col cols="12" sm="8" md="6">
      <div class="text-center">
        <logo />
        <vuetify-logo />
      </div>
      <v-card>
        <v-card-title class="headline">
          Welcome to our Vuetify + Nuxt.js integration app for Fiverr resources.
        </v-card-title>
        <v-card-text>
          <p>
            The goal of this app is to give our Fiverr resources a simple, clean
            way to build assets for us on a gig by gig basis.
          </p>
          <v-row>
            <v-col>How does it work?</v-col>
            <v-col
              >After we buy your gig, we send you the repo to fork. You can then
              create PR's (pull requests) off of the fork in github - just lik
              you're used to doing. Simply create the PR and we'll integrate the
              code then the gig is complete.</v-col
            >
          </v-row>
          <v-row>
            <v-col>How do we communicate?</v-col>
            <v-col
              >Per the Fiverr T&amp;C, we always communicate via Fiverr.</v-col
            >
          </v-row>
        </v-card-text>
        <v-row justify="center" align="center" class="ml-6">
          <v-col>
            <p>
              Thank you for developing with us and we can't wait to see what you
              create!!!
            </p>
          </v-col>
        </v-row>
      </v-card>
    </v-col>
  </v-row>
</template>

<script>
import Logo from '~/components/Logo.vue'
import VuetifyLogo from '~/components/VuetifyLogo.vue'

export default {
  components: {
    Logo,
    VuetifyLogo,
  },
}
</script>
