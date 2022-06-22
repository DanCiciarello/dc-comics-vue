<template>
    <div>
        <div class="bg-primary py-5">
            <div class="container text-white">
                <div class="d-flex">
                    <div class="col d-flex align-items-center" v-for="(item, i) in itemsFooter" :key="i">
                        <img :src="item.url" :alt="item.name" width="40">
                        <span class="cdFooterSpan text-uppercase ps-3">{{ item.name }}</span>
                    </div>
                </div>
            </div>
        </div>
    </div>
</template>

<!-- ------------------------ -->

<script>
export default {
    name: "BannerBlue",
    data(){
        return {
            itemsFooter: [
                {
                    name: "Digital Comics",
                    url: [require("../assets/img/buy-comics-digital-comics.png")],
                },
                {
                    name: "DC Merchandise",
                    url: [require("../assets/img/buy-comics-merchandise.png")],
                },
                {
                    name: "Subscription",
                    url: [require("../assets/img/buy-comics-subscriptions.png")],
                },
                {
                    name: "Comic Shop Locator",
                    url: [require("../assets/img/buy-comics-shop-locator.png")],
                },
                {
                    name: "DC Power Visa",
                    url: [require("../assets/img/buy-dc-power-visa.svg")],
                },
            ]
        }
    },
}
</script>

<!-- ------------------------ -->

<style lang="scss" scoped>

.cdFooterSpan {
    font-size: 13px;
    font-weight: 600;
}

</style>