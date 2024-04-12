<script>
import AppProplist from './AppProplist.vue';

export default {
    name: 'AppMainContent',
    components: {
        AppProplist
    },
}
</script>

<template>
<section>
    <div class="container p-4">
        <span class="top-left p-2 px-3">CURRENT SERIES</span>
        
        <AppProplist></AppProplist>
        <span class="p-2 px-3 bottom-center">LOAD MORE</span>
    </div>
</section>
</template>

<style scoped lang="scss">
@use '../style/partials/variables' as *;
section{
    background-color: $brand-secondary;
    .container{
        position: relative;
    }
        span{
            &.top-left{

                position: absolute;
                top:0;
                left: 0;
                transform: translateY(-50%);
            }
            &.bottom-center{
                position: absolute;
                bottom:10px;
                left: 50%;
                transform: translateX(-50%);
            }
            background-color: $brand-primary;
            color: white;
            font-weight: bold;
        
        }
}


</style>