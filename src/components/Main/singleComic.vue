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
    <div class="col-6 col-sm-4 col-md-3 col-lg-2 text-center text-white mt-4">
        <div class="image">
            <img :src="thumb" :alt="series">
        </div>
        <h6>{{series}}</h6>

        <span class="d-block">{{ type }}</span>
        <span class="d-block">{{ price }}</span>
    </div>
</template>

<style lang="scss" scoped>
.col-6 {
    &:hover {
        cursor: pointer;
        scale: 1.1 
    }
    img {
        height: 200px;
    }
}
</style>