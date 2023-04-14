<script>
export default {
    name: "singleComic",
    props: {
        thumb: String,
        price: String,
        series: String,
        type: String
    },
    data() {
        return {}
    }
}
</script>

<template>
    <div class="col-2 text-center text-white">
        <div class="image">
            <img :src="thumb" :alt="series">
        </div>
        <h6>{{series}}</h6>

        <span class="d-block">{{ type }}</span>
        <span class="d-block">{{ price }}</span>
    </div>
</template>

<style lang="scss" scoped>
.col-2 {
    img {
        height: 200px;
    }
}
</style>