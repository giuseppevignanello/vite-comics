<script>
export default {
    name: "bottomFooter",
    data () {
        
        return {
            socials: [
        {
          icon: "footer-facebook.png",
          link: "#"
        },
        {
          icon: "footer-periscope.png",
          link: "#"
        },
        {
          icon: "footer-pinterest.png",
          link: "#"
        },
        {
          icon: "footer-twitter.png",
          link: "#"
        },
        {
          icon: "footer-youtube.png",
          link: "#"
        },
      ]

        }
    },
     methods: {
   getImageUrl(name) {
  return new URL(`../../assets/img/${name}`, import.meta.url).href
} 
}
}
</script>

<template>
    <div id="bottom_footer">
      <div class="container d-flex justify-content-between py-3">
        <button class="sign_up_btn text-white p-2">
          SIGN UP NOW!
        </button>
        <div id="bottom_footer_right" class="d-flex align-items-center">
          <button class="follow_us_btn pe-1">
            <strong> FOLLOW US </strong>
          </button>
          <ul class="social d-flex mt-3">
            <li v-for="social in socials" class="me-2">
              <a :href="social.link">
                <img :src="getImageUrl(social.icon)" alt="">
              </a>
            </li>

          </ul>
        </div>
      </div>
    </div>

</template>

<style lang="scss" scoped>

</style>