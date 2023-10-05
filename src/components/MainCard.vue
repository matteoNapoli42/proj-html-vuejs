<script>
export default {
    name: "MainCard",
    props: {
        item: Object,
    }
}
</script>
<template>
    <div :class="$attrs.class">
        <img :src="item.img" alt="">
        <div :class="{ 'date_style': item.data !== undefined }">
            <span v-if="item.data !== undefined" class="date_padding mt-3">{{ item.data }}</span>
            <h4>{{ item.title }}</h4>
            <span>
                {{ item.message }}
            </span>
        </div>
    </div>
</template>

<style lang="scss">
@use '../assets/scss/partials/variables.scss' as *;

.wwdStyle {
    width: calc(100% / 12 * 4);
    margin-top: 53px;
}

.wwdStyle img {
    width: 80px;
    height: 78px;
    margin-bottom: 40px;
}

.wwdStyle h4 {
    margin-bottom: 15px;
}

.bestHStyle {
    width: calc((100% / 3) - 15px);
    margin-top: 53px;
}

.bestHStyle img {
    width: 100%;
}

.bestHStyle h4 {
    margin-top: 30px;
}

.teamStyle {
    width: calc((100% / 4) - 15px);
}

.teamStyle img {
    width: 100%;
    margin-top: 30px;
}

.teamStyle h4 {
    margin-top: 30px;
}

.articleStyle {
    width: calc((100% / 3) - 15px);
}

.articleStyle img {
    width: 100%;
    margin-top: 30px;
    text-align: left
}

.articleStyle h4 {
    margin-top: 10px;
    font-size: medium;
}

.articleStyle h4,
span {
    text-align: start;
}

h4 {
    font-weight: bold;
}

span {
    color: $cinema_tertiary;
}

.date_padding {
    padding-right: 55%;
}

.date_style {
    display: flex;
    flex-direction: column;
}
</style>