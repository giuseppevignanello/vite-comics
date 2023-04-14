<script>
import comics from "../data/comics.js"

export default {
    data() {
        return {
            comics: comics
        }
    },
  
}
</script>

<template>
    <div id="content" class="container">
        <div class="row">
            <div v-for="comic in comics" class="col-2">
                <img :src="comic.thumb" alt="">
            </div>
        </div>
    </div>
</template>

