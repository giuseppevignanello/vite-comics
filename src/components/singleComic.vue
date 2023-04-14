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
        <img :src="thumb" :alt="series">
        <h5>{{series}}</h5>
        <span class="d-block">{{type}}</span>
        <span class="d-block">{{price}}</span>
    </div>
</template>

<style lang="scss" scoped>

</style>