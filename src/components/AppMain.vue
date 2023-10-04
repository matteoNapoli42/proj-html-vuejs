<script>
import MainAbout from './MainAbout.vue';
import MainArticles from './MainArticles.vue';
import MainJumbo from './MainJumbo.vue';
import MainQuotes from './MainQuotes.vue';
import MainTeam from './MainTeam.vue';
import MainCard from './MainCard.vue';
import MainBestHits from './MainBestHits.vue';
import MainShowcase from './MainShowcase.vue';
import MainTech from './MainTech.vue';
import MainSubmit from './MainSubmit.vue';
import MainResult from './MainResult.vue';

export default {
    name: "AppMain",
    components: {
        MainJumbo,
        MainCard,
        MainAbout,
        MainBestHits,
        MainTeam,
        MainQuotes,
        MainArticles,
        MainShowcase,
        MainTech,
        MainSubmit,
        MainResult
    },
    data() {
        return {
            wwdItems: {

            }
        }
    }
}
</script>

<template>
    <!--Jumbotron-->
    <section id="jumbo" class=" px-2">
        <MainJumbo />
    </section>
    <section>
        <MainCard />
    </section>
    <section>
        <MainAbout />
    </section>
    <section>
        <MainBestHits />
    </section>
    <section>
        <MainResult />
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
