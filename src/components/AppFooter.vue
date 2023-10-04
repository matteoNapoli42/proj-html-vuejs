<script>
import UpperFooter from './UpperFooter.vue';
export default {
    name: "AppFooter",
    components: {
        UpperFooter,
    },
    data() {
        return {
            footerData: [
                {
                    title: "CONTACT INFO",
                    s1: "2/45 Tower Street, New York USA",
                    s2: "Call Us On 0800 840 1010",
                    s3: "Demo@Example.Com",
                    svg1: "src/assets/img/footer-location-dot-solid.svg",
                    svg2: "src/assets/img/footer-phone-solid.svg",
                    svg3: "src/assets/img/footer-envelope-soli.svg"
                }
            ]

        }
    }
}
</script>

<template>
    <div id="footer">
        <section class="container bg-danger h-100">
            <UpperFooter />
        </section>
        <!--
        <section class="row h-25" id="lowerFooter">
            <hr style="color: $cinema_tertiary; width: 80%;">
            <span class="text-centere">2023 All Rights Reserved. Developed by TemplateMela</span>
        </section>
        -->
    </div>
</template>

<style lang="scss">
@use '../assets/scss/partials/variables.scss' as *;

#footer {
    height: 560px;
    background-color: $cinema_secondary ;
}

#lowerFooter {
    color: $cinema_tertiary;
}
</style>
