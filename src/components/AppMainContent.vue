<script>
export default {
    name: 'AppMainContent',
    
}
</script>

<template>
<section>
    <div class="container p-4">
        <div class="content">------contento qui</div>
    </div>
</section>
</template>

<style scoped lang="scss">
@use '../style/partials/variables' as *;
section{
    background-color: $brand-secondary;
    .content{
        color: wheat;
    }
}


</style>