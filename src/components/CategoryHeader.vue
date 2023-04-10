<template>
  <div class="category-header">
    <h3>{{ title }}</h3>

    <div class="tabs">
      <div
        v-for="(tab, i) in tabs"
        class="tab"
        :class="{ active: activeIndex === i }"
        :key="tab"
        @click="activeIndex = i"
      >
        {{ tab }}
      </div>
    </div>
  </div>
</template>

<script setup>
import { ref } from 'vue';

defineProps({
  tabs: {
    type: [Array, Object]
  },
  title: {
    type: String
  }
})

const activeIndex = ref(0)

</script>

<style lang="scss" scoped>
.category-header {
  display: flex;
  justify-content: space-between;
  align-items: center;
  margin-bottom: 50px;

  h3 {
    font-weight: 600;
    font-size: 22px;
    line-height: 25px;
  }

  .tabs {
    display: flex;
    align-items: center;
    gap: 32px;

    @media(max-width: 969px){
      display: none;
    }
    .tab {
      font-weight: 600;
      font-size: 12px;
      line-height: 13px;
      opacity: 0.6;
      transition: 0.3s;
      cursor: pointer;
    }
    .active {
      opacity: 1;
    }
    :hover {
      opacity: 1;
    }
  }
}
</style>
