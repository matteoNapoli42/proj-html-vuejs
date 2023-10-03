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
        <a href="">
            {{ menuItem }}
            <img v-if="index == 2 || index == 6" src="src/assets/img/navDownArrow.svg" alt="" class="dropdown">
        </a>

    </li>
</template>
<style scoped>
.dropdown {
    width: 11px;
    height: 10px;
}

a {
    text-decoration: none;
    color: black;
}
</style>