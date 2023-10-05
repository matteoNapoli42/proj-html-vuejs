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
    <div class="d-flex align-items-center justify-content-between px-5" id="app_header">
        <div class="col-2 text-start">
            <img src="src/assets/img/logo.svg" alt="" style="width: 190px;">
        </div>
        <div class="col-4">
            <ul class="d-flex justify-content-between">
                <HeaderNav v-for="(elem, index) in navItems" :menuItem="elem" :index="index" />
            </ul>

        </div>
        <div class="col-2">
            <ul class="d-flex justify-content-around myP">
                <HeaderSocial v-for="(elem, index) in socialItems" :item="elem" :index="index" />
            </ul>

        </div>
    </div>
</template>

<style lang="scss" scoped>
@use '../assets/scss/partials/variables.scss' as *;

#app_header {
    background-color: $cinema_primary;
    height: 92px;

}

ul {
    list-style: none;
}

.myP {}
</style>

