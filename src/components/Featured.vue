<template>
    <section class="featured-products">
        <div class="container">
            <div class="products">

                <div class="product">
                    <div class="img-container">
                        <img src="@/assets/featured1.jpg" alt="">
                        <div class="content">
                            <h6>NOVA TEMPORADA</h6>
                            <h3>NOVA COLEÇÃO</h3>
                        </div>
                    </div>
                </div>

                <div class="product">
                    <div class="img-container">
                        <img src="@/assets/featured2.jpg" alt="">
                        <div class="content">
                            <h6>LIQUIDAÇÃO</h6>
                            <h3>ATÉ <span>50% DE DESCONTO</span></h3>
                        </div>
                    </div>
                </div>

            </div>
        </div>
    </section>
</template>

<script setup>

</script>

<style lang="scss" scoped>
.featured-products {
    margin-bottom: 90px;
    .container {
        .products{
            display: grid;
            grid-template-columns: 1fr 1fr;
            gap: 30px;
            .product {
                .img-container {
                    position: relative;
                    img {
                        object-fit: cover;
                    }
                    .content {
                        position: absolute;
                        top: 50%;
                        left: 50%;
                        transform: translate(-50%, -50%);
                        padding: 16px;
                        background-color: #ffffff;
                        text-align: center;
                        text-transform: uppercase;

                        h6 {
                            font-weight: 600;
                            font-size: 12px;
                            line-height: 13px;
                            opacity: 0.6;
                            margin-bottom: 6px;
                        }

                        h3 {
                            font-weight: 600;
                            font-size: 16px;
                            line-height: 18px;

                            span {
                                color: #E91E63;
                            }
                        }
                    }
                }
            }
        }
    }
}
</style>