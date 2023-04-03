<template>
    <div class="container">

        <div class="category-header">

            <h3>FEMININO</h3>

            <div class="tabs">
                <button
                    v-for="(tab, i) in tabs"
                    class="btn"
                    :class="{'active': activeIndex === i}"
                    :key="tab"
                    @click="activeIndex = i"
                    >
                        {{ tab }}
                </button>
            </div>

        </div>

        <div class="products">
            
            <div v-for="n in 6" :key="n" class="single-product">

                <div class="img-cont">
                    <img src="@/assets/femProducts/p1.png" alt="">
                </div>

                <div class="product-content">
                    <h6 class="name">Calça de treino feminina Q109</h6>
                    <div class="rating">
                        <span class="price">R$89,99</span>
                        <span class="icon">
                            <img src="@/assets/rating.png" alt="">
                        </span>
                    </div>
                </div>

            </div>

        </div>

        <button class="btn">Veja Todos</button>
            
    </div>
</template>

<script setup>
import { ref } from 'vue';


const tabs = ref([
    'Novidades',
    'Especiais',
    'Mais Vendidos',
    'Mais Vizualizados'
]);

const activeIndex = ref(0);

</script>

<style lang="scss" scoped>

.container {
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
    }
}



</style>