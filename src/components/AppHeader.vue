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
                "SHOP"//DROPDOWN index 7
            ],

            socialItems: [

            ],

        }
    }
}
</script>

<template>
    <div class="d-flex align-items-center justify-content-around px-5" id="app_header">
        <div class="col-3">
            asdfafa
        </div>
        <div class="col-6 ">
            <ul class="d-flex justify-content-evenly">
                <HeaderNav v-for="(elem, index) in navItems" :menuItem="elem" :index="index" />
            </ul>

        </div>
        <div class="col-3">
            <HeaderSocial />
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

