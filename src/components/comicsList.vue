<script>
import singleComic from "./singleComic.vue"
import comics from "../data/comics.js"
export default {
    components: {
        singleComic,
    },
    data() {
        return {
            comics: comics
        }
    },
  
}
</script>

<template>
    <div id="content" class="container py-5">
        <div class="row">
            <singleComic v-for="singleComic in comics" :thumb="singleComic.thumb" :series="singleComic.series" :price="singleComic.price" :type="singleComic.type"/>
        </div>
    </div>
</template>
