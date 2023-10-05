<script>
export default {
    name: "MainAbout"
}
</script>
<template>
    <div id="about" class="d-flex">
        <div class="col-6">

        </div>
        <div class="col-6 text-white d-flex flex-column gap-3" id="about-text">
            <span style=" color: white;">ABOUT US</span>
            <h1>HIGH QUALITY CINEMATICS</h1>
            <p style="line-height: 220%;">
                Lorem ipsum dolor sit amet consectetur adipisicing elit. Corrupti, et maxime enim laborum deserunt
                voluptatem
                quo eius, voluptate pariatur provident dolor quibusdam dolorem necessitatibus! Praesentium, aut rem. Nihil,
                voluptas iusto.
                Lorem ipsum dolor sit amet consectetur adipisicing elit. Provident ipsa rem dolore et, quam sint obcaecati,
                dolorem quibusdam nam, dolor unde odio cumque porro veniam quidem incidunt illo! Amet, ab.</p>
            <button class="btn btn-light w-25 py-2 rounded-0">READ MORE</button>
        </div>
    </div>
</template>
<style>
#about {
    height: 575px;
    background-image: url(src/assets/img/About-Us.jpg);
    background-size: cover;
    background-position: center;
}

#about-text {
    padding: 122px;
}
</style>