<script>
export default {
    name: "UpperFooter",
    props: {
        elem: Object,
    }

}
</script>

<template>
    <div class="col-3">
        <h3>{{ elem.title }}</h3>
        <span v-for="voice in elem.voices" class="d-flex footerElem">
            <img v-if="voice.img !== undefined" :src="voice.img" alt="">
            <span>{{ voice.text }}</span>
        </span>
    </div>
</template>
<style scoped>
img {
    height: 17px;
    width: 17px;
    margin-right: 10px;
}

.footerElem {
    margin-bottom: 24px;
}

h3 {
    text-align: start;
    margin-bottom: 28px;
}



span:hover {

    color: white;
}
</style>