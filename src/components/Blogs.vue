<template>
    <section class="blogs">
        <div class="container">

            <div class="blogs-header">
                <h3>Mais recente do blog</h3>
                <a href="#">Veja Tudo</a>
            </div>

            <div class="blogs-wrapper">

                <div class="blog">

                    <div class="img-container">
                        <img src="../assets/blog1.png" alt="">
                    </div>

                    <div class="blog-content">
                        <h3>Favoritos Recentes</h3>
                        <p>Lorem ipsum, dolor sit amet consectetur adipisicing elit. Quibusdam quae voluptatem commodi quisquam ducimus aut repellat est quasi, nesciunt beatae.</p>
                    </div>

                </div>

                <div class="blog">
                    
                    <div class="img-container">
                        <img src="../assets/blog2.png" alt="">
                    </div>

                    <div class="blog-content">
                        <h3>Temporada de Casamento</h3>
                        <p>Lorem ipsum, dolor sit amet consectetur adipisicing elit. Quibusdam quae voluptatem commodi quisquam ducimus aut repellat est quasi, nesciunt beatae.</p>
                    </div>

                </div>

                <div class="blog">
                    
                    <div class="img-container">
                        <img src="../assets/blog3.png" alt="">
                    </div>

                    <div class="blog-content">
                        <h3>Moda Casual Urbana</h3>
                        <p>Lorem ipsum, dolor sit amet consectetur adipisicing elit. Quibusdam quae voluptatem commodi quisquam ducimus aut repellat est quasi, nesciunt beatae.</p>
                    </div>

                </div>

            </div>

        </div>
    </section>
</template>

<script setup>

</script>

<style lang="scss" scoped>

.blogs {
    .container {
        .blogs-header {
           display: flex;
           justify-content: space-between;
           align-items: center;
           text-transform: uppercase;
           margin-bottom: 48px;

           h3 {
            font-weight: 600;
            font-size: 22px;
            line-height: 25px;
            color: #121212;
           }

           a {
            font-weight: 500;
            font-size: 12px;
            line-height: 13px;
            opacity: 0.6;
            color: #121212;
           }
        }

        .blogs-wrapper{
            display: grid;
            grid-template-columns: 1fr 1fr 1fr;
            gap: 30px;
            @media(max-width: 969px) {
                grid-template-columns: 1fr 1fr;
            }

            @media(max-width: 600px) {
                grid-template-columns: 1fr;
            }

            .blog {
                .blog-content {
                    max-width: calc(100% - 48px);
                    width: 100%;
                    margin: auto;
                    transform: translateY(-100px);
                    background: #FFFFFF;
                    padding: 24px 16px;
                    @media(max-width: 969px){
                        max-width: 100%;
                        transform: translateY(0px);
                    }
                    @media(max-width: 600px) {
                        padding: 10px 0px;
                    }
                }
            }
        }



    }
}

</style>