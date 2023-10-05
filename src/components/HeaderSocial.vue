<script>
export default {
    name: "HeaderSocial",
    props: {
        item: String,
        index: Number,
    }
}
</script>
<template>
    <li>
        <span v-if="index === 1" id="separator"></span>
        <a v-else href=""><img :src=item alt="" style="width: 21px; height: 22px;"></a>
    </li>
</template>
<style scoped>
#separator {
    height: 100%;
    border-right: 2px solid grey;
}
</style>