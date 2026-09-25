<script setup>
    import MainNavigation from './components/MainNavigation.vue';
    import SiteFooter from './components/SiteFooter.vue';
    import SiteContent from './components/SiteContent.vue';
</script>

<template>
    <header>
        <MainNavigation title="My Vue App" />
        <!-- <MainNavigation /> -->
    </header>

    <main>
        <SiteContent />
    </main>


    <footer>
        <!-- sitefooter komponens használata -->
        <SiteFooter />
    </footer>

</template>

<style scoped>
</style>
