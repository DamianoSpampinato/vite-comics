<script>
export default {
    name: 'Prop',
    props: {
        PropInfo: Object
    },
    methods: {
            getImageUrl(name) {
                return new URL(`${name}`, import.meta.url).href;
            }
        }
    
}
</script>

<template>

        <div class="col-2">
            <div class=" card">
                <div class="img-container">
                    <img :src="getImageUrl(PropInfo.thumb)" alt="">
                </div>
                <div class="text">{{ PropInfo.series.toUpperCase() }}</div>
            </div>

        </div>
  

</template>

<style scoped lang="scss">
.card{
    background-color: transparent;
    border: none;
    width: 100%;
    .img-container{
        height: 200px;
        width: 100%;
        overflow: hidden;
        img{
            width: 100%;
        }
    }
    .text{
        color:white
    }
}



</style>