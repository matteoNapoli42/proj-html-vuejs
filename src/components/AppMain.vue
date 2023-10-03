<script>
import MainAbout from './MainAbout.vue';
import MainArticles from './MainArticles.vue';
import MainJumbo from './MainJumbo.vue';
import MainQuotes from './MainQuotes.vue';
import MainTeam from './MainTeam.vue';
import MainWWD from './MainWWD.vue';
import MainBestHits from './MainBestHits.vue';
import MainShowcase from './MainShowcase.vue';
import MainTech from './MainTech.vue'
import MainSubmit from './MainSubmit.vue'

export default {
    name: "AppMain",
    components: {
        MainJumbo,
        MainWWD,
        MainAbout,
        MainBestHits,
        MainTeam,
        MainQuotes,
        MainArticles,
        MainShowcase,
        MainTech,
        MainSubmit
    }
}
</script>

<template>
    <!--Jumbotron-->
    <section id="jumbo" class=" px-2">
        <MainJumbo />
    </section>
    <section>
        <MainWWD />
    </section>
    <section>
        <MainAbout />
    </section>
    <section>
        <MainBestHits />
    </section>
    <section>
        <MainShowcase />
    </section>
    <section>
        <MainTeam />
    </section>
    <section>
        <MainQuotes />
    </section>
    <section>
        <MainArticles />
    </section>
    <section>
        <MainTech />
    </section>
    <section>
        <MainSubmit />
    </section>
</template>

<style lang="scss">
#jumbo {
    height: 800px;
    background-color: black;
}
</style>
