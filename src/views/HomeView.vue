<template>
    <div>
        <Banner />
        <ProductCategory :tabs="womenTabs" :title="womenTitle" :products="womenProducts" />
        <ProductCategory :tabs="menTabs" :title="menTitle" :products="menProducts" />
        <Featured />
        <Subscribe />
        <Blogs />
        <FooterComponent />
    </div>
</template>

<script setup>
import { ref } from 'vue'
import Banner from '../components/Banner.vue'
import ProductCategory from '../components/ProductCategory.vue'
import Featured from '../components/Featured.vue'
import Subscribe from '../components/Subscribe.vue'
import Blogs from '../components/Blogs.vue'
import FooterComponent from '../components/FooterComponent.vue'


const womenTabs = ref([
    'NOVIDADES',
    'ESPECIAIS',
    'MAIS VENDIDOS',
    'MAIS VISUALIZADOS'
])

const menTabs = ref([
    'NOVIDADES',
    'ESPECIAIS',
    'MAIS VENDIDOS',
    'MAIS VISUALIZADOS'
])

const womenTitle = ref('FEMININO')

const menTitle = ref('MASCULINO')

const womenProducts = ref([
    {
        img: "../assets/femProducts/p1.png",
        sale: false,
        name: "Calça de treino feminina Q109",
        price: "R$89,99",
        rating: "../assets/rating.png"
    },
    {
        img: "../assets/femProducts/p2.png",
        sale: true,
        name: "T-shirt básica estampada",
        price: "R$29,99",
        rating: "../assets/rating.png"
    },
    {
        img: "../assets/femProducts/p3.png",
        sale: false,
        name: "Sueter Branco",
        price: "R$69,99",
        rating: "../assets/rating.png"
    },
    {
        img: "../assets/femProducts/p4.png",
        sale: false,
        name: "Moletom Branco",
        price: "R$89,99",
        rating: "../assets/rating.png"
    },
    {
        img: "../assets/femProducts/p5.png",
        sale: false,
        name: "Sueter Cinza",
        price: "R$119,99",
        rating: "../assets/rating.png"
    },
    {
        img: "../assets/femProducts/p6.png",
        sale: false,
        name: "Calça Preta",
        price: "R$99,99",
        rating: "../assets/rating.png"
    },
    {
        img: "../assets/femProducts/p7.png",
        sale: false,
        name: "Calça Curta Feminina",
        price: "R$79,99",
        rating: "../assets/rating.png"
    },
    {
        img: "../assets/femProducts/p8.png",
        sale: true,
        name: "T-shirt Básica",
        price: "R$29,99",
        rating: "../assets/rating.png"
    }
])

const menProducts = ref([
    {
        img: "../assets/menProducts/p1.png",
        sale: false,
        name: "Moletom Masculino",
        price: "R$89,99",
        rating: "../assets/rating.png"
    },
    {
        img: "../assets/menProducts/p2.png",
        sale: true,
        name: "Calça Masculina",
        price: "R$79,99",
        rating: "../assets/rating.png"
    },
    {
        img: "../assets/menProducts/p3.png",
        sale: false,
        name: "Sueter Masculino Cinza",
        price: "R$119,99",
        rating: "../assets/rating.png"
    },
    {
        img: "../assets/menProducts/p4.png",
        sale: true,
        name: "Gorro Longo Cinza",
        price: "R$29,99",
        rating: "../assets/rating.png"
    },
    {
        img: "../assets/menProducts/p5.png",
        sale: false,
        name: "Moletom Bege",
        price: "R$119,99",
        rating: "../assets/rating.png"
    },
    {
        img: "../assets/menProducts/p6.png",
        sale: false,
        name: "Camisa Jeans",
        price: "R$99,99",
        rating: "../assets/rating.png"
    },
    {
        img: "../assets/menProducts/p7.png",
        sale: false,
        name: "Calça Fit Masculina",
        price: "R$99,99",
        rating: "../assets/rating.png"
    },
    {
        img: "../assets/menProducts/p8.png",
        sale: true,
        name: "Calça de Alfaiataria Cinza",
        price: "R$169,99",
        rating: "../assets/rating.png"
    }
])

</script>


<style scoped>
</style>
