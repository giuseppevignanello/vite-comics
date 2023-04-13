<script>
import appHeader from "./components/appHeader.vue"
export default {
  name:"App",
 components: {
  appHeader, 

 },
  data() {
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
      footerMenuItems:[
        {
          title: "DC COMICS",
          items: [
            "Lorem",
            "Lorem",
            "Lorem",
            "Lorem",
            "Lorem",
            "Lorem",
            "Lorem",
          ]
        },
        {
          title: "DC COMICS",
          items: [
            "Lorem",
            "Lorem",
            "Lorem",
            "Lorem",
            "Lorem",
            "Lorem",
            "Lorem",
            "Lorem",
            "Lorem",
            "Lorem",
          ]
        },
        {
          title: "DC COMICS",
          items: [
            "Lorem",
            "Lorem",
            "Lorem",
            "Lorem",
            "Lorem",
          ]
        },
        {
          title: "DC COMICS",
          items: [
            "Lorem",
            "Lorem",
            "Lorem",
          ]
        },
      ], 
      socials: [
        {
          icon: "src/assets/img/footer-facebook.png",
          link: "#"
        },
        {
          icon: "src/assets/img/footer-facebook.png",
          link: "#"
        },
        {
          icon: "src/assets/img/footer-facebook.png",
          link: "#"
        },
        {
          icon: "src/assets/img/footer-facebook.png",
          link: "#"
        },
        {
          icon: "./assets/img/footer-facebook.png",
          link: "#"
        },
      ]

    }
  }
}
</script>

<template>
 <appHeader/>
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
  <footer>
    <div id="top_footer">
      <div class="container d-flex">
        <div class="menu d-flex">
          <ul v-for="item in footerMenuItems">
            <li><h5>{{ item.title }}</h5></li>
            <li v-for="itemList in item.items">{{itemList}}</li>
            
        
          </ul>

        </div>
        <div class="logo">
          <img src="./assets/img/dc-logo-bg.png" alt="">
        </div>
      </div>
    </div>

    <div id="bottom_footer">
      <div class="container d-flex justify-content-between">
        <button class="btn">
          SIGN UP NOW
        </button>
        <ul class="social d-flex">
          <li>Follow US</li>
          <li v-for="social in socials">
            <a :href="social.link">
              <img :src="social.icon" alt="">
            </a>
          </li>
          
        </ul>
      </div>
    </div>

  </footer>
</template>

<style></style>
