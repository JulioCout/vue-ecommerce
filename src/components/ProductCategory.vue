<template>
    <div class="container">

        <CategoryHeader :tabs="tabs" :title="title"  />

        <div class="products">
            <SingleProduct v-for="(product, i) in products" :key="i" :product="products"/>
        </div>

        <button class="btn">Veja Todos</button>
            
    </div>
</template>

<script setup>
import { ref } from 'vue'
import SingleProduct from './SingleProduct.vue'
import CategoryHeader from './CategoryHeader.vue'


const tabs = ref([
    'NOVIDADES',
    'ESPECIAIS',
    'MAIS VENDIDOS',
    'MAIS VISUALIZADOS'
])

const title = ref('FEMININO')

const products = ref([
    {
        img: "@/assets/femProducts/p1.png",
        sale: false,
        name: "Calça de treino feminina Q109",
        price: "R$89,99",
        rating: "@/assets/rating.png"
    },
    {
        img: "@/assets/femProducts/p2.png",
        sale: true,
        name: "T-shirt básica estampada",
        price: "R$29,99",
        rating: "@/assets/rating.png"
    },
    {
        img: "@/assets/femProducts/p3.png",
        sale: false,
        name: "Sueter Branco",
        price: "R$69,99",
        rating: "@/assets/rating.png"
    },
    {
        img: "@/assets/femProducts/p4.png",
        sale: false,
        name: "Moletom Branco",
        price: "R$89,99",
        rating: "@/assets/rating.png"
    },
    {
        img: "@/assets/femProducts/p5.png",
        sale: false,
        name: "Sueter Cinza",
        price: "R$119,99",
        rating: "@/assets/rating.png"
    },
    {
        img: "@/assets/femProducts/p6.png",
        sale: false,
        name: "Calça Preta",
        price: "R$99,99",
        rating: "@/assets/rating.png"
    },
    {
        img: "@/assets/femProducts/p7.png",
        sale: false,
        name: "Calça Curta Feminina",
        price: "R$79,99",
        rating: "@/assets/rating.png"
    },
    {
        img: "@/assets/femProducts/p8.png",
        sale: true,
        name: "T-shirt Básica",
        price: "R$29,99",
        rating: "@/assets/rating.png"
    }
])

</script>

<style lang="scss" scoped>

.container {
    

    .products {
        display: grid;
        grid-template-columns: 1fr 1fr 1fr 1fr;
        gap: 30px;
    }
}
</style>