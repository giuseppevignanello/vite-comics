<script>
export default {
  name: "appMain",
  data() {
    return {
      footerMenuItems: [
        {
          title: "DC COMICS",
          items: [
            {
              title: "Characthers",
              link: "#"
            },
            {
              title: "Comics",
              link: "#"
            },
            {
              title: "Movies",
              link: "#"
            },
            {
              title: "TV",
              link: "#"
            },
            {
              title: "Games",
              link: "#"
            },
            {
              title: "Video",
              link: "#"
            },
            {
              title: "News",
              link: "#"
            }
          ]
        },
        {
          title: "DC",
          items: [
            {
              title: "Terms of Use",
              link: "#"
            },
            {
              title: "Privacy policy(New)",
              link: "#"
            },
            {
              title: "Ad Choices",
              link: "#"
            },
            {
              title: "Advertising",
              link: "#"
            },
            {
              title: "Jobs",
              link: "#"
            },
            {
              title: "Subscription",
              link: "#"
            },
            {
              title: "Talent Workshops",
              link: "#"
            },
            {
              title: "CPSC Certificates",
              link: "#"
            },
            {
              title: "Shop Help",
              link: "#"
            },
            {
              title: "Contact Us",
              link: "#"
            }
          ]
        },
        {
          title: "SITES",
          items: [
            {
              title: "DC",
              link: "#"
            },
            {
              title: "MAD MAGAZINE",
              link: "#"
            },
            {
              title: "DC Kids",
              link: "#"
            },
            {
              title: "DC Universe",
              link: "#"
            },
            {
              title: "DC Power VISA",
              link: "#"
            }
          ]
        },
        {
          title: "Shop",
          items: [
            {
              title: "Shop DC",
              link: "#"
            },
            {
              title: "Shop DC Collectibles",
              link: "#"
            }

          ]
        },
      ],
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
  return new URL(`../assets/img/${name}`, import.meta.url).href
} 
}
}
</script>

<template>
  <footer>
    <div id="top_footer">
      <div class="container d-flex">
        <div class="menu d-flex flex-wrap row-cols-3">
          <ul v-for="item in footerMenuItems">
            <li>
              <h5 class="title">{{ item.title }}</h5>
            </li>
            <li v-for="itemList in item.items">
              <a :href="itemList.link">{{ itemList.title }}</a>
            </li>


          </ul>

        </div>
      </div>
    </div>

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

  </footer>
</template> 