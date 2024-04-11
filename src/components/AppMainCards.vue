<script>
export default {
    name: 'AppMainCards',
    data(){
        return{
        cardsArray: [
            {
                title: 'digital comics',
                image: '../assets/img/buy-comics-digital-comics.png'
            },
            {
                title: 'dc merchandise',
                image: '../assets/img/buy-comics-merchandise.png'
            },{
                title: 'subscription',
                image: '../assets/img/buy-comics-subscriptions.png'
            },{
                title: 'comic shop locator',
                image: '../assets/img/buy-comics-shop-locator.png'
            },{
                title: 'dc power visa',
                image: '../assets/img/buy-dc-power-visa.svg'
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
<section id="card-section" class="p-3">
    <div class="container">
        <div class="row">
            <div v-for="card in cardsArray" class="col py-4">
                <div class="button d-flex justify-content-center align-items-center">
                    <div class="img-container">
                        <img :src="getImageUrl(card.image)" alt="">
                    </div>
                    <div class="text">{{ card.title.toUpperCase() }}</div>
                    
                </div>
            </div>
        </div>
        
    </div>
</section>
</template>

<style scoped lang="scss">
@use '../style/partials/variables' as *;
section{
    background-color: $brand-primary;
        .button{
            height: 100px;
            .img-container{
                height: 50%;
            }
            img{
                height: 100%;
            }
        }
    

    
    }



</style>