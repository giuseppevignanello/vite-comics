<script>
import comicsList from "./comicsList.vue"
export default {
  name: "appMain",
  components: {
    comicsList
  },
  data() {
    return {
      bandItems: [
        {
          img: "buy-comics-digital-comics.png",
          title: "DIGITAL COMICS"
        },
        {
          img: "buy-comics-merchandise.png",
          title: "DG MERCHANDISE"
        },
        {
          img: "buy-comics-subscriptions.png",
          title: "SUBSCRIPTION"
        },
        {
          img: "buy-comics-shop-locator.png",
          title: "COMIC SHOP LOCATOR"
        },
        {
          img: "buy-dc-power-visa.svg",
          title: "DC POWER VISA"
        },
      ],
 
    }

  },
  methods: {
    getImageUrl(name) {
      return new URL(`../assets/img/${name}`, import.meta.url).href
    }
  }
}
</script>

<template>
  <main>
   <comicsList/>
    <div id="band">
      <div class="container d-flex justify-content-between align-items-center">
        <div v-for="item in bandItems" class="icon d-flex align-items-center py-4">
          <img :src="getImageUrl(item.img)" alt="">
          <span class="text-white ms-3">{{ item.title }}</span>
        </div>
      </div>
    </div>
  </main>
</template> 

<style scoped lang="scss"></style>