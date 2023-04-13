<script>
export default {
    name: "appHeader",
    data(){
        return{
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
        <li class="col" v-for="item in menuItems">
          <a :href="item.link">{{ item.title }}</a>
        </li>
      </ul>
    </div>
  </header>
</template>


<style lang="scss" scoped>
</style>