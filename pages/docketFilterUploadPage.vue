<template>
  <EOComponentContainer
    title="Docket Filter Upload"
    :boundCpt="boundCtrl"
  ></EOComponentContainer>
</template>

<script>
import EOComponentContainer from '../components/EOComponentContainer.vue'
import DocketFilterUpload from '../components/DocketFilterUpload.vue'
export default {
  components: { EOComponentContainer },
  data() {
    return {
      boundCtrl: DocketFilterUpload,
    }
  },
}
</script>

<style>
</style>