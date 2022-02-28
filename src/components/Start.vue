<template>
    <div class="container vh-100 animate__animated animate__fadeInUpBig">
        <div class="row">
            <div class="col-md-8 about">
                <h1 class="animate__animated animate__bounce animate__delay-2s">hi, i'm Renan Leonel</h1>
                <p>i'm a <span class="animate__animated animate__bounce animate__delay-3s">front-end developer</span>  located in Brazil. i have huge interest on dynamic and intuitive web applications, using beautiful <span class="animate__animated animate__bounce animate__delay-4s">animations</span> and visual effects.</p>
                <p>currently working at <a class="work animate__animated animate__bounce animate__delay-5s" href="https://www.linkedin.com/company/cardano-warriors" target="_blank">Cardano Warriors</a> as a front-end developer intern.</p>
            </div>
            <div class="col-md-4 profilePic">
                <img class="img animate__animated animate__rollIn animate__delay-2s" src="../assets/renan_pixel.png" alt="Renan Leonel">
            </div>
        </div>
    </div>
</template>

<script>
export default {
    name: 'Start'
}
</script>

<style scoped>

    .container{
        display: flex;
        align-items: center;
    }
    .about{
        text-align: justify;
        text-justify: inter-word;
    }
    .profilePic{
        padding-left: 5rem;
    }
    .img{
        object-fit: contain;
        width: 15rem;
        border-radius: 1rem;
    }
    h1{
        padding-bottom: 2rem;
    }
    span, .work{
        display: inline-block;
    }
    span, h1, .work{
        font-weight: 700;
        color: #1664b1;
    }
    .work{
        text-decoration: none;
    }

    @media (max-width: 900px) {
        .profilePic{
            padding: 4rem 0 0 0;
            display: flex;
            justify-content: center;
        }

        h1{
            text-align: center;
        }
    }

    @media (max-width: 700px){
        .about{
            padding: 0 3rem;
        }
        h1{
            font-size: 1.5rem;
        }
        p{
            font-size: 1rem;
        }
    }
</style>