<template>
    <div class="background"> 
        <div class="container vh-100">
            <div class="row">
                <div class="headline">
                    <h3>currently working on more projects :)</h3>
                </div>
                <div class="col-md-5 img_warriors">
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

                <div class="col-md-5 img_portfolio offset-2">
                    <img class="portfolio" src="../assets/renan_pixel.png" alt="Cardano Warriors">
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
            </div>
        </div>
    </div>
</template>

<script>
    var portfolio = document.getElementsByClassName("img_portfolio")

    function resize(){
        if(window.matchMedia("(max-width:768px)").matches){
            for(let i = 0; i < portfolio.length; i++){
                portfolio[i].classList.remove('offset-2');
            }
        }
        else{
            for(let i = 0; i < portfolio.length; i++){
                portfolio[i].classList.add('offset-2');
            }
        }
    }

    window.onresize = function(){
        resize();
    }

    export default {
        name:"Projects"
    }
</script>

<style scoped>
    *{
        padding: 0;
    }
    .background{
        background-color: rgb(243, 243, 243);
    }
    .container{
        display: flex;
        align-items: center;
        justify-content: center;
    }
    .headline h3{
        font-weight: 400;
        color: #1664b1;
        font-family: 'Nanum Pen Script', cursive;
    }

    .warriors, .portfolio{
        width: 100%;
    }

    img{
        height: 25rem;
        border-radius: 1rem;
        object-fit: cover;
    }

    .stack{
        width: 100%;
        display: flex;
        justify-content: center;
        flex-direction: row;
        text-align: center;
    }

    .img_warriors, .img_portfolio{
        position: relative;
        border-radius: 1rem;
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

    @media (max-width: 800px) {
        .background{
            padding: 0 2rem;
        }

        img{
            height: 15rem;   
        }

        .row{
            padding: 0 2rem;
        }

        .image_title{
            font-size: 1.5rem;
        }

        .image_description, .stack{
            font-size: 1rem;
        }

        .stack{
            display: flex;
            justify-content: space-around;
        }
    }

    @media (max-width: 700px){
        h3{
        }
    }

</style>