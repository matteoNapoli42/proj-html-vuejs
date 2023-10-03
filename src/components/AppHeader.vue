<script>
import HeaderNav from './HeaderNav.vue';
import HeaderSocial from './HeaderSocial.vue';
export default {
    name: "AppHeader",
    components: {
        HeaderNav,
        HeaderSocial,
    },
    data() {
        return {
            navItems: [
                "HOME",
                "BLOG",
                "PAGES", //DROPDOWN index 2
                "ABOUT",
                "CONTACTS",
                "GALLERY",
                "SHOP",//DROPDOWN index 6
            ],

            socialItems: [
                "src/assets/img/navSearch.svg",
                "|",
                "src/assets/img/navFacebook.svg",
                "src/assets/img/navTwitter.svg",
                "src/assets/img/navYoutube.svg",
                "src/assets/img/navInstagram.svg",
            ]


        }
    }
}
</script>

<template>
    <div class="d-flex align-items-center justify-content-around px-5" id="app_header">
        <div class="col-3">
            <img src="src/assets/img/logo.svg" alt="" style="width: 190px;">
        </div>
        <div class="col-6 ">
            <ul class="d-flex justify-content-evenly">
                <HeaderNav v-for="(elem, index) in navItems" :menuItem="elem" :index="index" />
            </ul>

        </div>
        <div class="col-3">
            <ul class="d-flex justify-content-evenly">
                <HeaderSocial v-for="(elem) in socialItems" :item="elem" />
            </ul>

        </div>
    </div>
</template>

<style lang="scss">
@use '../assets/scss/partials/variables.scss' as *;

#app_header {
    background-color: $cinema_primary;
    height: 92px;

}

ul {
    list-style: none;
}
</style>

