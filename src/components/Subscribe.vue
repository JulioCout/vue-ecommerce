<template>
    <section class="subscribe-section">
        <div class="container">
            <div class="subscribe-wrapper">

                <h6>Oferta Especial</h6>

                <h3>Inscreva-se e <span>ganhe 10%</span> de desconto</h3>

                <input type="text" placeholder="E-mail">

                <button class="btn">Subscribe</button>

                <div class="img-container left">
                    <img src="../assets/subscribe-img-left" alt="">
                </div>

                <div class="img-container right">
                    <img src="../assets/subscribe-img-right.png" alt="">
                </div>
                
            </div>
        </div>
    </section>
</template>

<script setup>

</script>

<style lang="scss" scoped>
.subscribe-section {
    background: linear-gradient(180deg, #F3F2F2 0%, #DCDBDB 100%);
    .container {
        .subscribe-wrapper {
            max-width: 532px;
            width: 100%;
            margin: auto;
            background: #ffffff;
            position: relative;

            .img-container {
                position: absolute;
                top: 0;
                bottom: 0;
                left: 0;
                right: auto;
            }
        }
    }
}
</style>