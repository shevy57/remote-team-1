<template>
  <div>
    <v-row>
      <v-col>
        <img src="/v.png" alt="Vuetify.js" class="mb-5" />
      </v-col>
    </v-row>

    <v-row>
      <v-col>
        <blockquote class="blockquote">
          Welcome developer {{ devName }}!
        </blockquote>

        <span
          >Please complete your development here by replacing this class
          (EOWelcome) with your target class ({{ targetClass }})
        </span>
      </v-col>
    </v-row>
  </div>
</template>

<script>
export default {
  data() {
    return {
      devName: '',
      targetClass: 'DocketFilterUpload.Vue',
    }
  },
}
</script>

<style>
</style>