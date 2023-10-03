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
        <a href="" :class="[(index === 2 || index === 6) ? 'menuVoice' : '']">{{ menuItem }}</a>
    </li>
</template>
<style scoped>
.menuVoice::after {
    content: "<i class=" fa-solid fa-caret-down"></i>";
}

a {
    text-decoration: none;
    color: black;
}
</style>