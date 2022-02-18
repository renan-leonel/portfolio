<template>
    <div class="container vh-100">
        <div class="row vh-100">
            <div class="col-md-8 about">
                <h1>hi, i'm Renan Leonel</h1>
                <p>i'm a <span>front-end developer</span>  located in Brazil. i have huge interest on dynamic and intuitive web applications, using beautiful <span>animations</span> and visual effects.</p>
                <p>interested in the entire front-end ecosystem and researching about new <span>blockchain</span> and <span>web 3.0</span> technologies.</p>
                <p>currently working at <a class="work" href="https://www.linkedin.com/company/cardano-warriors" target="_blank">Cardano Warriors</a> as a front-end developer intern.</p>
            </div>
            <div class="col-md-4 profilePic">
                <img class="img" src="../assets/renan.jpg" alt="Renan Leonel">
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
    .row{
        display: flex;
        align-items: center;
    }
    .profilePic{
        padding-left: 5rem;
    }
    .img{
        object-fit: contain;
        width: 12rem;
        border-radius: 1rem;
    }
    span, h1, .work{
        font-weight: 700;
        color: #1664b1;
    }
    .work{
        text-decoration: none;
    }
</style>