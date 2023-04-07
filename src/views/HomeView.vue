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
        img: "https://i.imgur.com/OYQTjnB.png",
        sale: false,
        name: "Calça de treino feminina Q109",
        price: "R$89,99",
        rating: "../assets/rating.png"
    },
    {
        img: "https://i.imgur.com/gR999dy.png",
        sale: true,
        name: "T-shirt básica estampada",
        price: "R$29,99",
        rating: "../assets/rating.png"
    },
    {
        img: "https://i.imgur.com/LQXxco6.png",
        sale: false,
        name: "Sueter Branco",
        price: "R$69,99",
        rating: "../assets/rating.png"
    },
    {
        img: "https://i.imgur.com/EkjwbuD.png",
        sale: false,
        name: "Moletom Branco",
        price: "R$89,99",
        rating: "../assets/rating.png"
    },
    {
        img: "https://i.imgur.com/UL9axB3.png",
        sale: false,
        name: "Sueter Cinza",
        price: "R$119,99",
        rating: "../assets/rating.png"
    },
    {
        img: "https://i.imgur.com/SUlcDhh.png",
        sale: false,
        name: "Calça Preta",
        price: "R$99,99",
        rating: "../assets/rating.png"
    },
    {
        img: "https://i.imgur.com/5aliAOM.png",
        sale: false,
        name: "Calça Curta Feminina",
        price: "R$79,99",
        rating: "../assets/rating.png"
    },
    {
        img: "https://i.imgur.com/zW3WRvg.png",
        sale: true,
        name: "T-shirt Básica",
        price: "R$29,99",
        rating: "../assets/rating.png"
    }
])

const menProducts = ref([
    {
        img: "https://i.imgur.com/gsmBXBg.png",
        sale: false,
        name: "Moletom Masculino",
        price: "R$89,99",
        rating: "../assets/rating.png"
    },
    {
        img: "https://i.imgur.com/9lGNWvv.png",
        sale: true,
        name: "Calça Masculina",
        price: "R$79,99",
        rating: "../assets/rating.png"
    },
    {
        img: "https://i.imgur.com/yjMqacO.png",
        sale: false,
        name: "Sueter Masculino Cinza",
        price: "R$119,99",
        rating: "../assets/rating.png"
    },
    {
        img: "https://i.imgur.com/1IqyDaD.png",
        sale: true,
        name: "Gorro Longo Cinza",
        price: "R$29,99",
        rating: "../assets/rating.png"
    },
    {
        img: "https://i.imgur.com/YbJb3ks.png",
        sale: false,
        name: "Moletom Bege",
        price: "R$119,99",
        rating: "../assets/rating.png"
    },
    {
        img: "https://i.imgur.com/IXV1UEz.png",
        sale: false,
        name: "Camisa Jeans",
        price: "R$99,99",
        rating: "../assets/rating.png"
    },
    {
        img: "https://i.imgur.com/EkvKS8v.png",
        sale: false,
        name: "Calça Fit Masculina",
        price: "R$99,99",
        rating: "../assets/rating.png"
    },
    {
        img: "https://i.imgur.com/oufbcYK.png",
        sale: true,
        name: "Calça de Alfaiataria Cinza",
        price: "R$169,99",
        rating: "../assets/rating.png"
    }
])

</script>


<style scoped>
</style>
