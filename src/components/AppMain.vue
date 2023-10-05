<script>
import MainAbout from './MainAbout.vue';
import MainJumbo from './MainJumbo.vue';
import MainQuotes from './MainQuotes.vue';
import MainCard from './MainCard.vue';
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
        MainQuotes,
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
                    img: 'src/assets/img/Gallery-01.jpg',
                    title: 'SEVENTEENTH SUMMER',
                    message: 'Commercial Music Video',
                },

                {
                    img: 'src/assets/img/Gallery-02.jpg',
                    title: 'A MESSAGE TO SPACE',
                    message: 'Short Film',
                },

                {
                    img: 'src/assets/img/Gallery-03.jpg',
                    title: 'THE MOST BEAUTIFUL THING',
                    message: 'Music Video',
                },

                {
                    img: 'src/assets/img/Gallery-04.jpg',
                    title: 'PERMISSION TO SPEAK',
                    message: 'Documentary',
                },

                {
                    img: 'src/assets/img/Gallery-05.jpg',
                    title: 'EXPLORE OUR SPACE',
                    message: 'Film noir',
                },

                {
                    img: 'src/assets/img/Gallery-06.jpg',
                    title: 'FILM PRODUCTION',
                    message: 'Blaxploitation',
                },
            ],

            teamItems: [
                {
                    title: 'FABRICIO GUERRA',
                    message: 'Main Director',
                    img: 'src/assets/img/Team-01.jpg'
                },

                {
                    title: 'UMBERTO PAGODA',
                    message: 'Main Writer',
                    img: 'src/assets/img/Team-02.jpg'
                },

                {
                    title: 'GLORIA RICCASSO',
                    message: 'Main Producer',
                    img: 'src/assets/img/Team-03.jpg'
                },

                {
                    title: 'LIO NAPOIN',
                    message: 'Cameraman',
                    img: 'src/assets/img/Team-04.jpg'
                },
            ],

            articlesItems: [
                {
                    img: 'src/assets/img/article1.jpg',
                    title: 'RECAP YOUR LATEST COMPANY EVENT',
                    message: 'Suspendisse dictum dictum tempor. Ut non faucibus arcu, id elementum est. Suspendisse sed',
                },
                {
                    img: 'src/assets/img/article2.jpg',
                    title: 'HOW TO EDIT A FILM SCORE TO SERVE',
                    message: ' Lorem ipsum dolor sit amet consectetur adipisicing elit.',
                },
                {
                    img: 'src/assets/img/article3.jpg',
                    title: 'ARE YOU READY TO MAKE IT AWESOME',
                    message: 'Design is our playground. While we create an awesome experience, we like having fun. No animals',
                },
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
    <section class="text-center cardPadding" id="whatWD">
        <span>PELICULA STUDIO</span>
        <h1>THIS IS WHAT WE DO</h1>
        <div class="container d-flex flex-wrap">
            <MainCard v-for="(elem) in wwdItems" :item="elem" class="wwdStyle" />
        </div>
    </section>

    <section>
        <MainAbout />
    </section>

    <section class="text-center cardPadding" id="bestHits">
        <span>YOUR WATCHLIST</span>
        <h1>BEST HITS MOVIES</h1>
        <div class=" container d-flex flex-wrap justify-content-between">
            <MainCard v-for="(elem) in bestHItems" :item="elem" class="bestHStyle" />
        </div>
    </section>


    <section>
        <MainResult />
    </section>


    <section class="text-center cardPadding" id="team">
        <span>THE PERICUROS</span>
        <h1>MEET THE TEAM</h1>
        <div class=" container d-flex flex-wrap justify-content-between">
            <MainCard v-for="(elem) in  teamItems" :item="elem" class="teamStyle" />
        </div>

    </section>


    <section>
        <MainQuotes />
    </section>


    <section class="text-center cardPadding" id="articles">
        <span>LATEST NEWS</span>
        <h1>ARTICLES UPDATED DAILY</h1>
        <div class=" container d-flex flex-wrap justify-content-between">
            <MainCard v-for="(elem) in  articlesItems" :item="elem" class="articleStyle" />
        </div>
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
}

#bestHits {
    height: 1200px;
}

#team {
    height: 822px;
}

#articles {
    height: 800px;
}

.cardPadding {
    padding: 120px 0 120px 0;
}

span {
    font-size: small;
}
</style>
