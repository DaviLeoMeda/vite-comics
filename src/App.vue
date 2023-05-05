<script >
import DcHeader from './components/DcHeader.vue'
import DcMain from './components/DCmain.vue'
import DcFooter from './components/DcFooter.vue'

export default {
  name: "App",
  components: {
    DcHeader,
    DcMain,
    DcFooter
  }
}


</script>

<template>
  <DcHeader />
  <DcMain />
  <DcFooter />
</template>

<style lang="scss">
@use './style/main.scss';
@use './style/partials/_variables.scss';
</style>
