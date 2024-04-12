<script>
export default{
    name: 'AppHeader',
    data(){
        return{
            links: [
                {
                    text: 'characters',
                    status: false,
                },
                {
                    text: 'comics',
                    status: true,
                },
                {
                    text: 'movies',
                    status: false,
                },
                {
                    text: 'tv',
                    status: false,
                },
                {
                    text: 'games',
                    status: false,
                },
                {
                    text: 'collectibles',
                    status: false,
                },
                {
                    text: 'videos',
                    status: false,
                },
                {
                    text: 'fans',
                    status: false,
                },
                {
                    text: 'news',
                    status: false,
                },
                {
                    text: 'shop',
                    status: false,
                },
            ]
        }
    }
}
</script>
<template>
    <section class="header">
        <header class="">
            <div class="container d-flex justify-content-between align-items-center">
                <img src="../assets/img/dc-logo.png" alt="">
                <nav class="d-flex">

                    <a href="#" class="py-5" :class="{'active': link.status}" v-for="link in links">
                        {{ link.text.toUpperCase() }}
                    </a>
                </nav>
            </div>

            
        </header>
        
    </section>
</template>


<style scoped lang="scss">
@use '../style/partials/variables' as *;
nav{
    a{
        margin: 0 5px;
        text-decoration: none;
        color: black;
        
        &.active{
            border-bottom: 3px solid $brand-primary;
            color: $brand-primary;
            font-weight: bold;
            
            
        }
    
    }
    border: 10px black;
}


</style>