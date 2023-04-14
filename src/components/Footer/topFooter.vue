<script>
export default {
    name: "topFooter",
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
        }
    },
}
</script>

<template>
     <div id="top_footer" class="py-5">
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
</template>

<style lang="scss" scoped></style>