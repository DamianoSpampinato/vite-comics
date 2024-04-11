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
    }
}
    
</script>

<template>
<section id="card-section" class="p-3">
    <div class="container">
        <div class="row">
            <div v-for="card in cardsArray" class="col py-5">
                <div class="button d-flex">
                    <div class="img-container">
                        <img src="../assets/img/buy-dc-power-visa.svg" alt="">
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
            .img-container{
                width: 50px;
            }
            img{
                width: 100%;
            }
        }
    

    
    }



</style>