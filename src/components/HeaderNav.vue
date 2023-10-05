<script>
export default {
    name: "HeaderNav",
    props: {
        menuItem: String,
        index: Number,
    }
}
</script>
<template>
    <li>
        <a href="" :class="{ 'dropdown_navEl': index == 2 }">
            {{ menuItem }}
            <img v-if="index == 2 || index == 6" src="src/assets/img/navDownArrow.svg" alt="" class="dropdown">
            <div v-if="index == 2" class="dropdown_menu ">
                <ul>
                    <li><a href="">SERVICES</a></li>
                    <li><a href="">OUR WORK FLOW</a></li>
                    <li><a href="">VIDEO THUMBNAIL TYPE</a></li>
                </ul>
            </div>
        </a>

    </li>
</template>
<style  lang="scss" scoped>
.dropdown {
    width: 11px;
    height: 10px;
}

a {
    text-decoration: none;
    color: black;
}

.dropdown_navEl {}


.dropdown_navEl:hover {
    .dropdown_menu {
        display: block !important;
        z-index: 1 !important;
    }

}

.dropdown_menu {
    display: none;
    position: absolute;
    top: 7%;
    left: 43%;
    width: 250px;
    background-color: black;
    z-index: 1;
}

.dropdown_menu a {
    color: white;
}

.dropdown_menu ul {
    list-style: none;
    padding: 0;
}

.dropdown_menu li {
    list-style: none;
    border: 1px solid grey;
    padding: 5px 0px 10px 10px;
}
</style>