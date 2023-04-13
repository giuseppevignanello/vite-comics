<script>
export default {
  data() {
    return {
      menuItems: [
        {
          title: "comics",
          link:  "#"
        }, 
        {
          title: "comics",
          link:  "#"
        },
        {
          title: "comics",
          link:  "#"
        },
        {
          title: "comics",
          link:  "#"
        },
        {
          title: "comics",
          link:  "#"
        },
        {
          title: "comics",
          link:  "#"
        },
        {
          title: "comics",
          link:  "#"
        },
        {
          title: "comics",
          link:  "#"
        },
        {
          title: "comics",
          link:  "#"
        },
        {
          title: "comics",
          link:  "#"
        }
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
        <li class="col" v-for ="item in menuItems">
          <a :href="item.link">{{item.title }}</a>
        </li>
      </ul>
    </div>
  </header>
  <main>
    <div id="content" class="container">
      <h2 class="text-white pt-4">Content goes here</h2>
    </div>
    <div id="band">
      <div class="icon">
        <img src="./assets/img/buy-comics-digital-comics.png" alt="">
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
