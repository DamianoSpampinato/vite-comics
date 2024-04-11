<script>
import AppHeader from './components/AppHeader.vue';
import AppMainContent from './components/AppMainContent.vue';
import AppMainCards from './components/AppMainCards.vue';
export default{
    components:{
        AppHeader,
        AppMainContent,
        AppMainCards

    }
}

  
</script>

<template>
<AppHeader></AppHeader>
<AppMainContent></AppMainContent>
<AppMainCards></AppMainCards>

</template>

<style scoped>

</style>
