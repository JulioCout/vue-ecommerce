<script>
import Banner from '../components/Banner.vue';
import ProductCategory from '../components/ProductCategory.vue'

export default {
 name: "HomeView",
 components: {
    Banner,
    ProductCategory
 }
}
</script>

<template>
    <div>
        <Banner />
        <ProductCategory />
    </div>
</template>

<style scoped>
</style>
