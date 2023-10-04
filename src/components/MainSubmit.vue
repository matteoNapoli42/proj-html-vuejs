<script>
export default {
    name: "MainBestHits"
}
</script>
<template>
    <div id="submit">
        <div class="container d-flex gap-4">
            <div class="col-6 d-flex flex-column gap-3 myPT">
                <span>COLLABORATE</span>
                <h1>WANT TO WORK WITH US? <br> LEAVE US A MESSAGE!</h1>
                <p>
                    Lorem ipsum dolor sit amet consectetur adipisicing elit. Modi perferendis magni molestiae cumque
                    doloribus, illo iste. Non, expedita sequi nemo quisquam voluptate ullam assumenda qui? Unde asperiores a
                    aspernatur assumenda.</p>
            </div>
            <div class="col-6 myPT">
                <div class="d-flex flex-wrap  justify-content-between py-4">
                    <input type="name" placeholder="Your Name" class="formWidth border-0 bg-grey p-2 ">
                    <input type="mail" placeholder="Your Email" class="formWidth border-0 bg-grey  p-2 ">
                    <input type="text" placeholder="Mobile Number" class="formWidth  border-0 bg-grey  p-2 mt-5">
                    <input type="text" placeholder="Your Pincode" class="formWidth  border-0 bg-grey  p-2 mt-5">
                    <textarea class="col-12 mt-5 bg-grey border-0 p-2" placeholder="Enter Your Message"
                        style="min-height: 199px;"></textarea>
                    <button class="btn btn-dark col-12 mt-3 rounded-0">Submit Now</button>
                </div>


            </div>
        </div>
    </div>
</template>
<style lang="scss">
@use '../assets/scss/partials/variables.scss' as *;

#submit {
    height: 710px;
}

.bg-grey {
    background-color: $cinema_secondWhite;
}

.formWidth {
    width: calc(50% - 15px);
}

.myPT {
    padding-top: 90px;
}
</style>