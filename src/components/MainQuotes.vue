<script>
export default {
    name: "MainQuotes"
}
</script>
<template>
    <div id="quotes">
        <div class="container text-center myPY">
            <img src='src/assets/img/image (20).svg' alt="" id="svgStyle">
            <p>
                Lorem ipsum dolor sit amet consectetur adipisicing elit. Incidunt maxime dolorum magni, ullam aut fugiat
                totam laudantium possimus quia maiores ducimus ipsa quae ea vel doloremque iste! Dignissimos, eum
                qui?
            </p>
            <div class="d-flex justify-content-center gap-2">
                <img src="src/assets/img/01.jpg" class=" rounded-5" alt="" id="teamMember">
                <div class="">
                    <h6>JOHN DOE</h6>
                    <span>Designer</span>
                </div>

            </div>
        </div>
    </div>
</template>
<style>
#quotes {
    height: 600px;
    background-image: url(src/assets/img/Parallax-02.jpg);
    background-position-y: -37%;
    color: white;
}

.myPY {
    padding-top: 155px;
}

#svgStyle {
    height: 47px;
    width: 52px;
    filter: invert(100%);
    margin-bottom: 47px;
}
</style>