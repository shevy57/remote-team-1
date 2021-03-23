<template>
  <v-row justify="center" align="center">
    <v-col cols="12" sm="8" md="6">
      <div class="text-center">
        <logo />
        <vuetify-logo />
      </div>
      <v-card>
        <v-card-title class="headline">
          <p>
            Welcome to our Vuetify + Nuxt.js integration app for Fiverr
            resources.
          </p>
        </v-card-title>
        <v-card-text>
          <v-row>
            <v-col>
              <span class="text-subtitle-1 blue--text text--lighten-2">
                The goal of this app is to give our Fiverr resources a simple,
                clean way to build assets for us on a gig-by-gig basis.
              </span>
            </v-col>
          </v-row>

          <v-row>
            <v-col>How does it work?</v-col>
            <v-col
              >After we buy your gig, we send you the repo to fork. You can then
              create PR's (pull requests) off of the fork in github - just like
              you're used to doing.
              <p>Simply create the PR and we'll integrate the code.</p></v-col
            >
          </v-row>
          <v-row>
            <v-col>What if I've never done this before?</v-col>
            <v-col>
              <p>
                If you've never done a Fork/PR before on github, don't worry!
                It's easy. Just watch this short video and you'll be a pro in no
                time!
              </p>
              <p>
                <a href="https://tinyurl.com/yn6zfhx2"
                  >How to contribute on github</a
                >
              </p>
            </v-col>
          </v-row>
        </v-card-text>
        <v-row justify="center" align="center" class="ml-6">
          <v-col sm="6">
            <span class="red--text"> &hearts;&hearts;&hearts; </span>
            <span class="green--text text--lighten-3">
              Thank you for developing with us - we can't wait to see what you
              create!!!
            </span>
            <span class="red--text"> &hearts;&hearts;&hearts; </span>
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
