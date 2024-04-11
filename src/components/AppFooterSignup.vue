<script>
export default {
    name: 'AppFooterSignup',
    data(){
        return{
        images: [
            {
    
                image: '../assets/img/footer-facebook.png'
            },
            {
                
                image: '../assets/img/footer-twitter.png'
            },{
            
                image: '../assets/img/footer-youtube.png'
            },{
                
                image: '../assets/img/footer-pinterest.png'
            },{
            
                image: '../assets/img/footer-periscope.png'
            },
        ]
        
        
        }
    },
    methods: {
            getImageUrl(name) {
                return new URL(`${name}`, import.meta.url).href;
            }
        }
    
}
</script>

<template>
<section id="footer-links">
    <div class="container d-flex justify-content-between align-items-center p-3">
        <button>SIGN-UP NOW</button>
        <div class="follow-us d-flex">
            <div class="text d-flex align-items-center">Follow US</div>
            <div v-for="image in images" class="img-container m-2">
                <img :src="getImageUrl(image.image)" alt="">
            </div>
        </div>
    </div>
</section>
</template>

<style scoped lang="scss">
@use '../style/partials/variables' as *;
section{
    background-color: #303030;
    button{
        background-color: transparent;
        border: 2px solid $brand-primary;
        padding: 7px;
        color: white;
        font-weight: bold;
    }
    .text{
        color: $brand-primary;
        font-weight: bold;
      
    }
}

</style>