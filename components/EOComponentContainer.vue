<template>
  <v-card :light="!dark" minHeight="600">
    <v-toolbar :color="bar.class" :light="!dark">
      <v-app-bar-nav-icon></v-app-bar-nav-icon>
      <v-toolbar-title>{{ title }}</v-toolbar-title>
      <v-spacer></v-spacer>
      <v-switch v-model="dark" class="mt-5"></v-switch>
      <v-btn icon>
        <v-icon>mdi-heart</v-icon>
      </v-btn>
    </v-toolbar>
    <v-card :light="!dark" class="mt-8" elevation="0">
      <v-row>
        <v-col class="text-center">
          <EOWelcome></EOWelcome>
        </v-col>
      </v-row>

      <v-row>
        <v-col class="text-center">
          <component v-bind:is="boundCpt"></component>
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
  props: {
    title: {
      type: String,
      default: 'Title',
    },
    boundCpt: {
      type: Object,
      default: () => {},
    },
  },
}
</script>

<style>
</style>