<script>

import AppHeader from './components/AppHeader.vue';
import AppMainContent from './components/AppMainContent.vue';
import AppMainCards from './components/AppMainCards.vue';
import AppFooterLinks from './components/AppFooterLinks.vue';
import AppFooterSignup from './components/AppFooterSignup.vue';
import AppJumbo from './components/AppJumbo.vue';
export default{
    components:{
        AppHeader,
        AppMainContent,
        AppMainCards,
        AppFooterLinks,
        AppFooterSignup,
        AppJumbo

    }
}

</script>

<template>
<AppHeader></AppHeader>
<main>
    <AppJumbo></AppJumbo>
    <AppMainContent></AppMainContent>
    <AppMainCards></AppMainCards>
    <AppFooterLinks></AppFooterLinks>
    <AppFooterSignup></AppFooterSignup>
</main>
    
</template>

<style lang="scss">
@use './style/generic' as *;
</style>
