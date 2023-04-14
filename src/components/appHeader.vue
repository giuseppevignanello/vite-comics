<script>
export default {
  name: "appHeader",
  data() {
    return {
      activeMenuItem: -1,
      menuItems: [
        {
          title: "CHARACTERS",
          link: "#"
        },
        {
          title: "COMICS",
          link: "#"
        },
        {
          title: "MOVIES",
          link: "#"
        },
        {
          title: "TV",
          link: "#"
        },
        {
          title: "GAMES",
          link: "#"
        },
        {
          title: "COLLECTIBLES",
          link: "#"
        },
        {
          title: "VIDEOS",
          link: "#"
        },
        {
          title: "FANS",
          link: "#"
        },
        {
          title: "NEWS",
          link: "#"
        },
        {
          title: "SHOP",
          link: "#"
        }
      ],
    }
  }, 
  methods: {
    activeMenu(index) {
      this.activeMenuItem = index; 

    }
  }
}
</script>
<template>
  <header class="container d-flex justify-content-between py-3 align-items-center">
    <div class="logo">
      <img src="../assets/img/dc-logo.png" alt="">
    </div>
    <div class="menu">
      <ul class="row">
        <li @click="activeMenu(index)" class="col" :class="index ===activeMenuItem ? 'active' : ''" v-for="(item, index) in menuItems">
          <a :href="item.link">{{ item.title }}</a>
        </li>
      </ul>
    </div>
  </header>
  <section class="jumbotron">

  </section>
</template>


<style lang="scss" scoped>
.active {
  background-color: lightgray;
}
</style>