<script>
export default {
  data() {
    return {
      menuItems: [
        {
          title: "comics",
          link: "#"
        },
        {
          title: "comics",
          link: "#"
        },
        {
          title: "comics",
          link: "#"
        },
        {
          title: "comics",
          link: "#"
        },
        {
          title: "comics",
          link: "#"
        },
        {
          title: "comics",
          link: "#"
        },
        {
          title: "comics",
          link: "#"
        },
        {
          title: "comics",
          link: "#"
        },
        {
          title: "comics",
          link: "#"
        },
        {
          title: "comics",
          link: "#"
        }
      ],
      bandItems: [
        {
          img: "./assets/img/buy-comics-digital-comics.png",
          title: "DIGITAL COMICS"
        },
        {
          img: "./assets/img/buy-comics-digital-comics.png",
          title: "DIGITAL COMICS"
        },
        {
          img: "./assets/img/buy-comics-digital-comics.png",
          title: "DIGITAL COMICS"
        },
        {
          img: "./assets/img/buy-comics-digital-comics.png",
          title: "DIGITAL COMICS"
        },
        {
          img: "./assets/img/buy-comics-digital-comics.png",
          title: "DIGITAL COMICS"
        },
      ]

    }
  }
}
</script>

<template>
  <header class="container d-flex justify-content-between py-3">
    <div class="logo">
      <img src="./assets/img/dc-logo-bg.png" alt="">
    </div>
    <div class="menu">
      <ul class="row">
        <li class="col" v-for="item in menuItems">
          <a :href="item.link">{{ item.title }}</a>
        </li>
      </ul>
    </div>
  </header>
  <main>
    <div id="content" class="container">
      <h2 class="text-white pt-4">Content goes here</h2>
    </div>
    <img src="" alt="">
    <div id="band">
      <div class="container d-flex">
        <div v-for="item in bandItems" class="icon">
          <img src="" alt="">
          <h6 class="text-white">{{ item.title }}</h6>
        </div>
      </div>
    </div>
  </main>
  <footer>
    <div id="top_footer">

    </div>

    <div id="bottom_footer">

    </div>

  </footer>
</template>

<style></style>
