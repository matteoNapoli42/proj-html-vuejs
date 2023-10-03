<script>
export default {
    name: "HeaderSocial",
    props: {
        item: String,
    }
}
</script>
<template>
    <li>
        <a href=""><img :src=item alt="" style="width: 21px; height: 22px;"></a>
    </li>
</template>
<style></style>