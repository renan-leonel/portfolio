<template>
    <div class="container vh-100">
        <div class="row">
            <div class="col-md-8 about">
                <h1>hi, i'm Renan Leonel</h1>
                <p>i'm a <span>front-end developer</span>  located in Brazil. i have huge interest on dynamic and intuitive web applications, using beautiful <span>animations</span> and visual effects.</p>
                <p>currently working at <a class="work" href="https://www.linkedin.com/company/cardano-warriors" target="_blank">Cardano Warriors</a> as a front-end developer intern.</p>
            </div>
            <div class="col-md-4 profilePic">
                <img class="img" src="../assets/renan_pixel.png" alt="Renan Leonel">
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
    span, h1, .work{
        font-weight: 700;
        color: #1664b1;
    }
    .work{
        text-decoration: none;
    }

    @media (max-width: 850px) {
        .profilePic{
            padding: 4rem 0 0 0;
            display: flex;
            justify-content: center;
        }
    }
</style>