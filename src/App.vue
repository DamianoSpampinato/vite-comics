<script>

import AppHeader from './components/AppHeader.vue';
import AppMainContent from './components/AppMainContent.vue';
import AppMainCards from './components/AppMainCards.vue';
import AppFooterLinks from './components/AppFooterLinks.vue';
export default{
    components:{
        AppHeader,
        AppMainContent,
        AppMainCards,
        AppFooterLinks

    }
}

</script>

<template>
<AppHeader></AppHeader>
<AppMainContent></AppMainContent>
<AppMainCards></AppMainCards>
<AppFooterLinks></AppFooterLinks>

</template>

<style lang="scss">
@use './style/generic' as *;
</style>
