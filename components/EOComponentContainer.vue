<template>
  <v-card :light="!dark">
    <v-toolbar :color="bar.class" :light="!dark">
      <v-app-bar-nav-icon></v-app-bar-nav-icon>
      <v-toolbar-title>Title</v-toolbar-title>
      <v-spacer></v-spacer>
      <v-switch v-model="dark" class="mt-5"></v-switch>
      <v-btn icon>
        <v-icon>mdi-heart</v-icon>
      </v-btn>
    </v-toolbar>
    <v-card :light="!dark" class="mt-8" elevation="0">
      <v-row>
        <v-col class="text-center">
          <img src="/v.png" alt="Vuetify.js" class="mb-5" />
          <blockquote class="blockquote">
            Container for docket filter upload
            <footer>
              <small>
                <em>&mdash;John Johnson</em>
              </small>
            </footer>
          </blockquote>
        </v-col>
      </v-row>
    </v-card>
  </v-card>
</template>

<script>
export default {
  computed: {
    computedDark() {
      return !!this.dark
    },
  },
  data() {
    return {
      bar: {
        class: null,
      },
      dark: false,
    }
  },
}
</script>

<style>
</style>