<template>
  <div>
    <v-banner class="text-left" elevation="3" single-line>
      <v-icon slot="icon" color="info" size="36"> mdi-account-voice </v-icon>
      <v-row>
        <v-col cols="6">
          <blockquote class="blockquote">
            Welcome developer {{ devName }}! Please complete your development
            here by updating the target file (
            <span class="blue--text">{{ targetClass }} </span>)
          </blockquote>
        </v-col>
      </v-row>
    </v-banner>
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