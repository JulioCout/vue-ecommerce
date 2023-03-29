<script>
//import { RouterLink, RouterView } from 'vue-router'
import HeaderComp from './components/HeaderComp.vue';

export default {
  name: "app",
  components: {
    HeaderComp
  }
}

</script>

<template>
  <HeaderComp />

  <RouterView />
</template>

<style scoped>
</style>
