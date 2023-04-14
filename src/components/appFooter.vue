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
          icon: "src/assets/img/footer-facebook.png",
          link: "#"
        },
        {
          icon: "src/assets/img/footer-periscope.png",
          link: "#"
        },
        {
          icon: "src/assets/img/footer-pinterest.png",
          link: "#"
        },
        {
          icon: "src/assets/img/footer-twitter.png",
          link: "#"
        },
        {
          icon: "src/assets/img/footer-youtube.png",
          link: "#"
        },
      ]

    }

  }
}
</script>

<template>
  <footer>
    <div id="top_footer">
      <div class="container d-flex">
        <div class="menu d-flex">
          <ul v-for="item in footerMenuItems">
            <li>
              <h5>{{ item.title }}</h5>
            </li>
            <li v-for="itemList in item.items">
              <a :href="itemList.link">{{ itemList.title }}</a>
            </li>


          </ul>

        </div>
        <div class="logo">
          <img src="../assets/img/dc-logo-bg.png" alt="">
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

</footer></template> 