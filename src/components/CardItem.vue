<template>
    <div>
        <div class="cdThumbImg">
            <img :src="serie.thumb" alt="serie.series">
            <div class="card-img-overlay">
                <p class="card-text">
                    <span class="cdInnerTitle">
                        PRICE:
                    </span>
                    <br>
                    {{ serie.price }}
                </p>
                <p class="card-text">
                    <span class="cdInnerTitle">
                        TYPE:
                    </span>
                    <br>
                    {{ serie.type }}
                </p>
            </div>
        </div>
        <div>
            <span class="cdThumbTitle text-uppercase text-white">{{ serie.series }}</span>
        </div>
    </div>
</template>

<!-- ------------------------ -->

<script>
export default {
    name: "CardItem",
    props: {
        serie: Object,
    }
}
</script>

<!-- ------------------------ -->

<style lang="scss" scoped>

.cdThumbImg {
    width: 100%;
    aspect-ratio: 1/1;
    overflow: hidden;
    position: relative;

    &:hover .card-img-overlay {
        display: unset;
    }

    .card-img-overlay {
        padding: 20px 20px;
        background-color: rgba($color: #000000, $alpha: .8);
        color: #ffffff;
        display: none;

        .cdInnerTitle {
            font-size: 14px;
            font-weight: 600;
        }
    }

}

.cdThumbTitle {
    display: inline-block;
    font-size: 13px;
    font-weight: 600;
    margin-top: 15px;
    margin-bottom: 40px;
}

</style>