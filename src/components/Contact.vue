<template>
    <div class="contact">
        <div class="row contact">
            <h3 class="text1">you can find me here:</h3>
            <div class="links">
                <a href="https://www.linkedin.com/in/renanleonel/" target="_blank"><i class="fa-brands fa-linkedin"></i></a>
                <a href="https://github.com/renan-leonel" target="_blank"><i class="fa-brands fa-github"></i></a>
                <a href="mailto:renanleonelpro@gmail.com" target="_blank"><i class="fa-brands fa-google"></i></a>
            </div>
            <h3 class="text2">it will be a pleasure to answer your questions</h3>
        </div>
    </div>
</template>

<script>
export default {
    name: 'Contact'
}
</script>

<style scoped>
    .contact{
        background-color: rgb(243, 243, 243);
    }
    .contact{
        text-align: center;
    }
    .text1{
        margin: 10rem 0 5rem 0;
    }
    .text2{
        margin: 5rem 0 10rem 0;
    }

    a{
        font-size: 3rem;
        padding: 0 1rem;
        text-decoration: none;
        color: inherit;
    }

    @media (max-width: 760px) {
        .contact{
            padding: 0 2rem;
        } 
    }
</style>