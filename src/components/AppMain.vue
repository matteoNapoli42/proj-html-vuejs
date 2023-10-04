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
            wwdItems: [
                {
                    img: 'src/assets/img/wwdCamera.svg',
                    title: 'ARRAY OF EQUIPMENT',
                    message: 'Lorem ipsum dolor sit amet consectetur adipisicing elit. Pellentesque ultricies justa tellus.'
                },

                {
                    img: 'src/assets/img/wwdGlasses.svg',
                    title: 'NEW TECHNOLOGIES',
                    message: 'Lorem ipsum dolor sit amet consectetur adipisicing elit. Pellentesque ultricies justa tellus.',
                },

                {
                    img: 'src/assets/img/wwdMask.svg',
                    title: 'VERSITILE ACTORS',
                    message: 'Lorem ipsum dolor sit amet consectetur adipisicing elit. Pellentesque ultricies justa tellus.',
                },

                {
                    img: 'src/assets/img/wwdChair.svg',
                    title: 'TOP DIRECTORS',
                    message: 'Lorem ipsum dolor sit amet consectetur adipisicing elit. Pellentesque ultricies justa tellus.',
                },

                {
                    img: 'src/assets/img/wwdCiak.svg',
                    title: 'MINUTE EDITING',
                    message: 'Lorem ipsum dolor sit amet consectetur adipisicing elit. Pellentesque ultricies justa tellus.',
                },

                {
                    img: 'src/assets/img/wwdFilm.svg',
                    title: 'VERSITILE ACTORS',
                    message: 'Lorem ipsum dolor sit amet consectetur adipisicing elit. Pellentesque ultricies justa tellus.',
                }
            ],

            bestHItems: [
                {

                }
            ]
        }
    }
}
</script>

<template>
    <!--Jumbotron-->
    <section id="jumbo" class=" px-2">
        <MainJumbo />
    </section>


    <!--What We DO-->
    <section class="text-center" id="whatWD">
        <span>PELICULA STUDIO</span>
        <h1>THIS IS WHAT WE DO</h1>
        <div class="container d-flex flex-wrap">
            <MainCard v-for="(elem) in wwdItems" :item="elem" class="wwdStyle" />
        </div>
    </section>

    <section>
        <MainAbout />
    </section>


    <section class="" id=" bestHits">
        <MainBestHits />
    </section>


    <section>
        <MainResult />
    </section>


    <section class="" id="team">
        <MainTeam />
    </section>


    <section>
        <MainQuotes />
    </section>


    <section id="articles">
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

#whatWD {
    height: 824px;
    padding-top: 121px;
}

#bestHits {
    height: 1200px;
    background-color: violet;
}

#team {
    height: 822px;
    background-color: aqua;
}

#articles {
    height: 800px;
    background-color: salmon;
}
</style>
