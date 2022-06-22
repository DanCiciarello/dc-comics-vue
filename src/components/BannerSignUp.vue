<template>
    <div>
        <div class="bg-dark py-4">
            <div class="container text-white">
                <div class="d-flex justify-content-between">
                    
                    <!-- First column -->
                    <div>
                        <a href="#" class="cdBtnCta">
                            Sign-up now!
                        </a>
                    </div>

                    <!-- Second column -->
                    <div class="d-flex align-items-center">
                        <h5 class="text-primary text-uppercase">Follow us</h5>
                        <div v-for="(social, i) in imgFooter" :key="i">
                            <a href="#"><img class="cdFooterImg" :src="social.url" :alt="social.name"></a>
                        </div>
                    </div>

                </div>
            </div>
        </div>
    </div>
</template>

<!-- ------------------------ -->

<script>

export default {
    name: "BannerSignUp",
    data(){
        return {
            imgFooter: [
                {
                    name: "Facebook",
                    url: [require("../assets/img/footer-facebook.png")],
                },
                {
                    name: "Twitter",
                    url: [require("../assets/img/footer-twitter.png")],
                },
                {
                    name: "Youtube",
                    url: [require("../assets/img/footer-youtube.png")],
                },
                {
                    name: "Pinterest",
                    url: [require("../assets/img/footer-pinterest.png")],
                },
                {
                    name: "Periscope",
                    url: [require("../assets/img/footer-periscope.png")],
                }
            ]
        }
    },
}

</script>

<!-- ------------------------ -->

<style lang="scss" scoped>

.cdFooterImg {
    padding-left: 10px;
}

</style>