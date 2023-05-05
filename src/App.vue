<script >
import DcHeader from './components/DcHeader.vue'
import DcMain from './components/DCmain.vue'

export default {
  name: "App",
  components: {
    DcHeader,
    DcMain
  }
}


</script>

<template>
  <DcHeader />
  <DcMain />
</template>

<style lang="scss">
@use './style/main.scss';
@use './style/partials/_variables.scss';
</style>
