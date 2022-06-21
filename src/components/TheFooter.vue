<template>
    <div>
        <div class="cdFooter">
            <div class="container text-white">
                <div class="row">

                    <!-- First column -->
                    <div class="col-1 py-4">
                        
                        <!-- DC Comics menu -->
                        <h6 class="text-uppercase">DC Comics</h6>
                        <ul class="list-unstyled pb-4">
                            <li v-for="(item, i) in dcComicsMenu" :key="i">
                                <a class="text-reset text-decoration-none" :href="item.href">
                                {{ item.name }}
                                </a>
                            </li>
                        </ul>

                        <!-- Shop menu -->
                        <h6 class="text-uppercase">Shop</h6>
                        <ul class="list-unstyled">
                            <li v-for="(item, i) in shopMenu" :key="i">
                                <a class="text-reset text-decoration-none" :href="item.href">
                                {{ item.name }}
                                </a>
                            </li>
                        </ul>

                    </div>

                    <!-- Second column -->
                    <div class="col-1 py-4">
                        
                        <!-- DC menu -->
                        <h6 class="text-uppercase">DC</h6>
                        <ul class="list-unstyled pb-4">
                            <li v-for="(item, i) in dcMenu" :key="i">
                                <a class="text-reset text-decoration-none" :href="item.href">
                                {{ item.name }}
                                </a>
                            </li>
                        </ul>

                    </div>

                    <!-- Third column -->
                    <div class="col-1 py-4">
                        
                        <!-- DC menu -->
                        <h6 class="text-uppercase">Sites</h6>
                        <ul class="list-unstyled pb-4">
                            <li v-for="(item, i) in sitesMenu" :key="i">
                                <a class="text-reset text-decoration-none" :href="item.href">
                                {{ item.name }}
                                </a>
                            </li>
                        </ul>

                    </div>

                    <!-- Logo column -->
                    <div class="col-9 d-flex justify-content-end">
                        <img src="../assets/img/dc-logo-bg.png" alt="Logo DC" class="cdFooterImg">
                    </div>

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
    background-size: contain;
    overflow: hidden;

    .cdFooterImg {
        transform: translateY(-5%);
        position: absolute;
    }
}

</style>