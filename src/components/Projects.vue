<template>
    <div class="container vh-100">
        <div class="headline">
            <h1>Projects</h1>
        </div>
        <div class="row mainSection">
            <div class="col-md img_warriors">
                <img class="warriors" src="../assets/warriors.png" alt="Cardano Warriors">
                <div class="image_overlay">
                    <div class="image_title">Cardano Warriors</div>
                    <p class="image_description">Worked in the development of the main website for the play-to-earn NFT game Cardano Warriors</p>
                    <div class="stack">
                        
                        <p class="col-md-6">
                            <i class="fa-brands fa-vuejs"></i>
                            Vue.js
                        </p>
                        <p class=" col-md-6">
                            <i class="fa-brands fa-bootstrap"></i>
                            Bootstrap
                        </p>
                    </div>
                </div>
            </div>
        </div>
        <div class="row others">
            <div class="col-md img_portfolio">
                <img class="warriors" src="../assets/portfolio.png" alt="Portfolio">
                <div class="image_overlay">
                    <div class="image_title">Portfolio</div>
                    <p class="image_description">Created to practice my skills in web development</p>
                    <div class="stack">
                        
                        <p class="col-md-6">
                            <i class="fa-brands fa-vuejs"></i>
                            Vue.js
                        </p>
                        <p class=" col-md-6">
                            <i class="fa-brands fa-bootstrap"></i>
                            Bootstrap
                        </p>
                    </div>
                </div>
            </div>
            <div class="col-md img_opense">
                <img class="warriors" src="../assets/opense.png" alt="Portfolio">
                <div class="image_overlay">
                    <div class="image_title">Open-SE</div>
                    <p class="image_description">My first ever website, using simple HTML and CSS for the Workshop on Open Science Practices for Software Engineering</p>
                    <div class="stack">
                        <p class="col-md-6">
                            <i class="fa-brands fa-html5"></i>
                            HTML
                        </p>
                        <p class=" col-md-6">
                            <i class="fa-brands fa-css3"></i>
                            CSS
                        </p>
                    </div>
                </div>
            </div>
        </div>
    </div>
</template>

<script>
export default {
    name:"Projects"
}
</script>

<style scoped>
    *{
        padding: 0;
    }

    .headline h1{
        font-weight: 700;
        color: #1664b1;
        padding-bottom: 4rem;
    }

    .warriors{
        display: block;
        width: 100%;
    }

    img{
        height: 30rem;
        border-radius: 1rem;
        object-fit: cover;
    }

    .stack{
        width: 50%;
        display: flex;
        justify-content: center;
        flex-direction: row;
        text-align: center;
    }

    .img_warriors, .img_portfolio, .img_opense{
        width: 100%;
        position: relative;
        border: 1px solid #bebebe;
        border-radius: 1rem;
    }

    .img_warriors{
        margin-bottom: 4rem;
    }
    .img_portfolio{
        margin-right: 2rem;
    }
    .img_opense{
        margin-left: 2rem;
    }
    .others{
        margin-bottom: 4rem;
    }

    /* image overlay effects */
    .image_overlay{
        width: 100%;
        height: 100%;
        
        position: absolute;
        top: 0;
        left: 0;

        display: flex;
        flex-direction: column;
        align-items: center;
        justify-content: center;

        background: rgba(0, 0, 0, 0.8);
        color: #ffffff;
        border-radius: 1rem;
        opacity: 0;
        transition: opacity 0.5s;
    }

    .image_overlay:hover{
        opacity: 1;
    }

    .image_overlay > *{
        transform : translateY(2rem);
        transition: transform 0.25s;
    }

    .image_overlay:hover > *{
        transform : translateY(0);
    }

    .image_title{
        font-size: 2rem;
        margin-top: 0.25rem;
    }

    .image_description{
        width: 75%;
        text-align: center;
        font-size: 1.25rem;
        margin-top: 0.25rem;
    }
</style>