<script>
export default {
    name: "appMain",
    data(){
        return {
            bandItems: [
        {
          img: "src/assets/img/buy-comics-digital-comics.png",
          title: "DIGITAL COMICS"
        },
        {
          img: "src/assets/img/buy-comics-digital-comics.png",
          title: "DIGITAL COMICS"
        },
        {
          img: "src/assets/img/buy-comics-digital-comics.png",
          title: "DIGITAL COMICS"
        },
        {
          img: "src/assets/img/buy-comics-digital-comics.png",
          title: "DIGITAL COMICS"
        },
        {
          img: "src/assets/img/buy-comics-digital-comics.png",
          title: "DIGITAL COMICS"
        },
      ],
        }
  
    }
}
</script>

<template> 
<main>
    <div id="content" class="container">
      <h2 class="text-white pt-4">Content goes here</h2>
    </div>
    <img src="" alt="">
    <div id="band">
      <div class="container d-flex">
        <div v-for="item in bandItems" class="icon">
          <img :src="item.img" alt="">
          <h6 class="text-white">{{ item.title }}</h6>
        </div>
      </div>
    </div>
  </main>
</template> 