<template>
  <HeaderComp />
  <RouterView />
</template>


<script setup>

//import { RouterLink, RouterView } from 'vue-router'

import HeaderComp from './components/HeaderComp.vue';

</script>

<style>

.container {
  max-width: calc(144opx - 170px);
  width: 100%;
  margin: auto;
}

.btn {
  background: transparent;
  border: none;
  transition: 0.3s;
  cursor: pointer;
  width: 100%;
  display: flex;
  justify-content: center;
  align-items: center;
}

</style>
