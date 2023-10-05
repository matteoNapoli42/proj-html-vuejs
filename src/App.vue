<script>
import AppHeader from './components/AppHeader.vue';
import AppMain from './components/AppMain.vue';
import AppFooter from './components/AppFooter.vue';
export default {
    name: "App",
    components: {
        AppHeader,
        AppMain,
        AppFooter
    }


}
</script>

<template>
    <header>
        <AppHeader />
    </header>

    <main class="p-left">
        <AppMain />
    </main>

    <footer>
        <AppFooter />
    </footer>
</template>

<style scoped >
.p-left {
    padding-left: 13px;
}
</style>
