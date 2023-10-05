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

.articleStyle {}
</style>