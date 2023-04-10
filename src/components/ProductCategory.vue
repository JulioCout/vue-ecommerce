<template>
    <section class="product-category">
        <div class="container">
    
            <CategoryHeader :tabs="tabs" :title="title"  />
    
            <div class="products">
                <SingleProduct v-for="(product, i) in products" :key="i" :product="product"/>
            </div>
    
            <button class="btn">Veja Todos</button>
                
        </div>
    </section>

</template>

<script setup>
import SingleProduct from './SingleProduct.vue'
import CategoryHeader from './CategoryHeader.vue'

defineProps(['title', 'products', 'tabs'])

</script>

<style lang="scss" scoped>

.product-category {
    margin-bottom: 100px;

    .container {
        .products {
            display: grid;
            grid-template-columns: 1fr 1fr 1fr 1fr;
            gap: 30px;
            @media (max-width: 969px) {
                grid-template-columns: 1fr 1fr;
            }
            @media (max-width: 400px) {
                grid-template-columns: 1fr;
            }
        }
        .btn {
            height: 48px;
            background: #F8F8F8;
            border: 2px solid #F8F8F8;
            max-width: 100%;
            margin-top: 18px;
        }
    }
}





</style>