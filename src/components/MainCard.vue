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
        <h4>{{ item.title }}</h4>
        <span>
            {{ item.message }}
        </span>
    </div>
</template>

<style>
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

.bestHStyle {}

.teamStyle {}

.articleStyle {}
</style>