<script>

import AppHeader from './components/AppHeader.vue';
import AppMainContent from './components/AppMainContent.vue';
import AppMainCards from './components/AppMainCards.vue';
import AppFooterLinks from './components/AppFooterLinks.vue';
import AppFooterSignup from './components/AppFooterSignup.vue';
export default{
    components:{
        AppHeader,
        AppMainContent,
        AppMainCards,
        AppFooterLinks,
        AppFooterSignup

    }
}

</script>

<template>
<AppHeader></AppHeader>
<AppMainContent></AppMainContent>
<AppMainCards></AppMainCards>
<AppFooterLinks></AppFooterLinks>
<AppFooterSignup></AppFooterSignup>

</template>

<style lang="scss">
@use './style/generic' as *;
</style>
