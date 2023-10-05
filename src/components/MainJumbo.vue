<script>
export default {
    name: "MainJumbo",
}
</script>
<template>
    <div id="carouselExample" class="carousel slide h-100">
        <div class="carousel-inner h-100">
            <div class="carousel-item active" id="item1">
                <div class=" car-text h-100 col-6 w-100 d-flex align-items-center justify-content-evenly ">
                    <div class="col-1">
                        <button class="btn_color">
                            <img src="src/assets/img/left-arrow.svg" alt="" class="arrow">
                        </button>
                    </div>

                    <div class="col-8">
                        <h5>CINEMATO STUDIO</h5>
                        <h1>ACTION AND <br> INSPIRE PEOPLE</h1>
                        <button class="btn btn-light px-4 rounded-0 mt-3">READ MORE</button>
                    </div>
                    <div class="col-1 text-end">
                        <button class="btn_color"><img src="src/assets/img/right-arrow.svg" alt="" class="arrow">
                        </button>
                    </div>


                </div>
            </div>
        </div>
    </div>
</template>
<style scoped>
img {
    max-height: 750px;
}

.car-text {
    padding: 257px 0 257px 0;
}

#item1 {
    background-image: url('src/assets/img/Gallery-01.jpg');
    background-size: cover;
    background-repeat: no-repeat;
    height: 100%;
    margin-right: 1.3px;
    color: white;
}

h1 {
    font-size: 300%;
}

.btn_color {
    background-color: #231d1f;
    width: 39px;
    height: 39px;
}

.arrow {
    width: 14px;
    height: 16px;

    filter: invert(100%);
}
</style>