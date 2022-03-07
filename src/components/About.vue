<template>
    <div class="container">
        <div class="row vh-100">
            <div class="col-md-8 about">
                <h2>about me</h2>
                <p>Hi! I'm in my last year at university at <span>State University of Maringá</span> and mainly focusing on my internship and personal projects.</p>
                <p>I'm also interested in the entire front-end ecosystem and researching about new <span>blockchain</span> and <span>web 3.0</span> technologies.</p>
                <p>In my free time, i love playing fantasy games <span class="likes">(big soulsborne fan here)</span> and reading.</p>
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
    p{
        text-align:justify;
        text-justify: inter-character;
    }
    span, h2{
        font-weight: 700;
        color: #1664b1;
    }
    h2{
        padding-bottom: 4rem;
    }
    .likes{
        font-weight: 200;
        color: #8f8f8f;
        font-family: 'Nanum Pen Script', cursive;;
    }
    @media (max-width: 900px) {
        .container{
            padding: 0 2rem;
        }

        .profilePic{
           display: none;
        }

        h2{
            padding-bottom: 2rem;
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