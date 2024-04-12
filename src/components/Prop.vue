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
                    <img class="comic-image" :src="getImageUrl(PropInfo.thumb)" alt="">
                </div>
                <div class="text">{{ PropInfo.series.toUpperCase() }}</div>
            </div>

        </div>
  

</template>

<style scoped lang="scss">
.card{
    background-color: transparent;
    border: none;
    height: 100%;
    width: 100%;
    .img-container{
        height: 80%;
        width: 200px;
        overflow: hidden;
        .comic-image{
            width: 100%;
            object-fit: cover;
            height: 100%;
            
        }
    }
    .text{
        color:white
    }
}



</style>