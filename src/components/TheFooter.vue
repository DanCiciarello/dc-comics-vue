<template>
    <div>
        <div class="cdFooter">
            <div class="container text-white">
                <div class="d-flex">

                    <!-- First column -->
                    <div class="cdCol">
                        
                        <!-- DC Comics menu -->
                        <h5 class="text-uppercase">DC Comics</h5>
                        <ul class="list-unstyled pb-4">
                            <li v-for="(item, i) in dcComicsMenu" :key="i">
                                <a class="text-reset text-decoration-none cdFooterMenuItem" :href="item.href">
                                {{ item.name }}
                                </a>
                            </li>
                        </ul>

                        <!-- Shop menu -->
                        <h5 class="text-uppercase">Shop</h5>
                        <ul class="list-unstyled">
                            <li v-for="(item, i) in shopMenu" :key="i">
                                <a class="text-reset text-decoration-none cdFooterMenuItem" :href="item.href">
                                {{ item.name }}
                                </a>
                            </li>
                        </ul>

                    </div>

                    <!-- Second column -->
                    <div class="cdCol">
                        
                        <!-- DC menu -->
                        <h5 class="text-uppercase">DC</h5>
                        <ul class="list-unstyled pb-4">
                            <li v-for="(item, i) in dcMenu" :key="i">
                                <a class="text-reset text-decoration-none cdFooterMenuItem" :href="item.href">
                                {{ item.name }}
                                </a>
                            </li>
                        </ul>

                    </div>

                    <!-- Third column -->
                    <div class="cdCol">
                        
                        <!-- DC menu -->
                        <h5 class="text-uppercase">Sites</h5>
                        <ul class="list-unstyled pb-4">
                            <li v-for="(item, i) in sitesMenu" :key="i">
                                <a class="text-reset text-decoration-none cdFooterMenuItem" :href="item.href">
                                {{ item.name }}
                                </a>
                            </li>
                        </ul>

                    </div>

                    <!-- Logo column -->
                    <div class="cdColImg flex-grow-1 d-flex justify-content-end"></div>

                </div>
            </div>
        </div>
    </div>
</template>

<!-- ------------------------ -->

<script>

export default {
    name: "TheFooter",
    data(){
        return {
            dcComicsMenu: [
                {
                    name: "Characters",
                    href: "#"
                },
                {
                    name: "Comics",
                    href: "#"
                },
                {
                    name: "Movies",
                    href: "#"
                },
                {
                    name: "TV",
                    href: "#"
                },
                {
                    name: "Games",
                    href: "#"
                },
                {
                    name: "Collectibles",
                    href: "#"
                },
                {
                    name: "Videos",
                    href: "#"
                },
                {
                    name: "Fans",
                    href: "#"
                },
                {
                    name: "News",
                    href: "#"
                },
            ],
            shopMenu: [
                {
                    name: "Shop DC",
                    href: "#"
                },
                {
                    name: "Shop DC Collectibles",
                    href: "#"
                },
            ],
            dcMenu: [
                {
                    name: "Terms of Use",
                    href: "#"
                },
                {
                    name: "Privacy Policy (New)",
                    href: "#"
                },
                {
                    name: "Ad Choices",
                    href: "#"
                },
                {
                    name: "Advertising",
                    href: "#"
                },
                {
                    name: "Jobs",
                    href: "#"
                },
                {
                    name: "Subscription",
                    href: "#"
                },
                {
                    name: "Talent Workshops",
                    href: "#"
                },
                {
                    name: "CPSC Certificates",
                    href: "#"
                },
                {
                    name: "Ratings",
                    href: "#"
                },
                {
                    name: "Shop Help",
                    href: "#"
                },
                {
                    name: "Contact Us",
                    href: "#"
                },
            ],
            sitesMenu: [
                {
                    name: "DC",
                    href: "#"
                },
                {
                    name: "Mad Magazine",
                    href: "#"
                },
                {
                    name: "DC Kids",
                    href: "#"
                },
                {
                    name: "DC Universe",
                    href: "#"
                },
                {
                    name: "DC Power Visa",
                    href: "#"
                },
            ],
        }
    }
}

</script>

<!-- ------------------------ -->

<style lang="scss" scoped>

.cdFooter {
    background-image: url("../assets/img/footer-bg.jpg");
    background-size: cover;

    .cdCol {
        width: 150px;
        padding: 30px 0;
    }

    .cdColImg {
        background-image: url("../assets/img/dc-logo-bg.png");
        background-repeat: no-repeat;
        background-position: center right;
    }

    .cdFooterMenuItem {
        font-size: 12px;
        color: grey!important;
    }
}

</style>