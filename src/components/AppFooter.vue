<script>
import UpperFooter from './UpperFooter.vue'
export default {
    name: "AppFooter",
    components: {
        UpperFooter,
    },
    data() {
        return {
            footerData: [
                {
                    title: 'CONTACT INFO',
                    voices: [
                        {
                            img: 'src/assets/img/footer-location-dot-solid.svg',
                            text: '2/45 Tower Street, New York USA'
                        },
                        {
                            img: 'src/assets/img/footer-phone-solid.svg',
                            text: 'Call US On 0800 840 1010',
                        },
                        {
                            img: 'src/assets/img/footer-envelope-soli.svg',
                            text: 'Demo@Example.Com',
                        }

                    ]
                },
                {
                    title: 'INFORMATION',
                    voices: [
                        {
                            text: 'Product Support',
                        },

                        {
                            text: 'Checkout',
                        },

                        {
                            text: 'Report Abuse',
                        },

                        {
                            text: 'Redeem Voucher',
                        },

                        {
                            text: 'Order Status'
                        }
                    ]
                },

                {
                    title: 'USEFUL LINKS',
                    voices: [
                        {
                            text: 'Policies & Rules',
                        },

                        {
                            text: 'Privacy Policy',
                        },

                        {
                            text: 'License Policy',
                        },

                        {
                            text: 'My Account',
                        },

                        {
                            text: 'Locality',
                        }
                    ]
                }
            ]

        }
    }
}
</script>

<template>
    <div id="footer">
        <section class="container d-flex">
            <UpperFooter v-for="elem in footerData" :elem="elem" />
            <div class="col-3 text-start">
                <h3 style="margin-bottom: 53px;">NEWSLETTER</h3>
                <div class=" d-flex flex-column gap-2">
                    <span>Subscribe To Receive Inspiration, Idead & News In Your Inbox</span>
                    <div class="d-flex flex-column mt-5 gap-2">
                        <input class="w-75 border-0 p-2 mb-1" type="text" placeholder="Enter Your Email">
                        <button class="btn btn-light rounded-0 p-2 w-50"> SUBSCRIBE</button>
                    </div>
                </div>
            </div>
        </section>

        <section class="row" id="lowerFooter">
            <hr style="color: $cinema_tertiary; width: 80%;">
            <span class="text-center">2023 All Rights Reserved. Developed by TemplateMela</span>
        </section>
    </div>
</template>

<style lang="scss" scoped>
@use '../assets/scss/partials/variables.scss' as *;

#footer {
    height: 560px;
    background-color: $cinema_secondary ;
    color: $cinema_secondWhite;
    padding-top: 111px;
}

#lowerFooter {
    color: $cinema_tertiary;
    margin-top: 120px;
}

input {
    margin-bottom: 10px;
    background-color: #1c1c1c;
}
</style>
