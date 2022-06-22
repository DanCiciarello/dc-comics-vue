<template>
    <div>
        <div class="cdThumbImg">
            <img :src="serie.thumb" alt="serie.series">
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
}

.cdThumbTitle {
    display: inline-block;
    font-size: 13px;
    font-weight: 600;
    margin-top: 15px;
    margin-bottom: 40px;
}

</style>