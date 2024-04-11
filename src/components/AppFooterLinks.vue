<script>
export default {
    name: 'AppFooterLinks',
    
}
</script>

<template>
<section id="footer-links">
    <div class="container">
        <div class="row">
            <div class="col-4">Lorem ipsum, dolor sit amet consectetur adipisicing elit. Magnam, asperiores! Perspiciatis pariatur dolor nobis ipsam, cumque, incidunt, doloremque quidem quia ipsa autem sapiente aliquam maiores voluptas sint blanditiis asperiores! Nemo.</div>
            <div class="col-8 d-flex"><img src="../assets/img/dc-logo-bg.png" alt=""></div>
        </div>
    </div>
</section>
</template>

<style scoped lang="scss">
section{
    background-image: url('../assets/img/footer-bg.jpg');
    background-size: cover;
    height: 500px;
    .container{
        height: 100%;
        .row{
            height: 100%;
        }
    }
    .col-8{
        height: 100%;
    
        overflow-y: hidden;
    
        img{
            height: 120%;
            transform: translateY(-10%);
            
         
        }

    }
}


</style>