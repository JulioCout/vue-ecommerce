<template>
    <section class="subscribe-section">
        <div class="container">
            <div class="subscribe-wrapper">

                <h6>Oferta Especial</h6>

                <h3>Inscreva-se e ganhe <span>10% de desconto</span></h3>

                <input type="text" placeholder="E-mail">

                <button class="btn">Subscribe</button>

                <div class="img-container left">
                    <img src="../assets/subscribe-img-left.png" alt="">
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
    padding: 60px 0px;
    overflow-y: hidden;
    margin-bottom: 50px;
    @media(max-width: 600){
                margin: 60px 20px;
            }
    .container {
        .subscribe-wrapper {
            max-width: 532px;
            width: 100%;
            margin: auto;
            background: #ffffff;
            position: relative;
            text-align: center;
            padding: 80px 0px;
            text-transform: uppercase;
            @media(max-width: 969px){
                padding: 80px 20px;
            }
            @media(max-width: 600px){
                padding: 80px 20px;
            }

            h6 {
                font-weight: 600;
                font-size: 12px;
                line-height: 13px;
                opacity: 0.4;
            }

            h3 {
                font-weight: 700;
                font-size: 26px;
                line-height: 36px;
                max-width: 300px;
                text-align: center;
                margin: auto;
                margin-bottom: 32px;

                span {
                    color: #E91E63;
                }
                @media(max-width: 400px){
                    font-size: 16px;
                    line-height: 20px;
                }
            }

            input {
               height: 50px; 
               max-width: 340px;
               margin: auto;
               background: #F8F8F8;
               text-align: center;
               border: none;
               outline: none;
               width: 100%;
               margin-bottom: 20px;
               border-radius: 5px;
               @media(max-width: 400px){
                    height: 40px;
                }
            }

            .btn {
                height: 64px; 
                max-width: 340px;
                background: #121212;
                border: 2px solid #121212;
                margin: auto;
                font-weight: 500;
                font-size: 16px;
                line-height: 18px;
                color: #FFFFFF;
                text-transform: uppercase;
                opacity: 0.9;
                border-radius: 5px;
                @media(max-width: 400px){
                    height: 40px;
                }
            }

            .img-container {
                position: absolute;
                top: 0;
                bottom: 0;
                left: -50%;
                right: auto;
                @media(max-width: 969px){
                    display: none;
                }
            }

            .right {
                height: 100px;
                left: auto;
                right: -32%;

                img {
                    height: 450px;
                }
            }

            .left {
                height: 584px;
            }
        }
    }
}
</style>