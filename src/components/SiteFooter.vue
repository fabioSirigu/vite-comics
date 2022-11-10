<script>
export default {
      name: 'SiteFooter',
      data() {
            return {
                  DcComics: [
                        {
                              text: 'Characters'
                        },
                        {
                              text: 'Comics'
                        },
                        {
                              text: 'Movies'
                        },
                        {
                              text: 'TV'
                        },
                        {
                              text: 'Games'
                        },
                        {
                              text: 'Videos'
                        },
                        {
                              text: 'News'
                        }
                  ],
                  Shop: [
                        {
                              text: 'Shop DC'
                        },
                        {
                              text: 'Shop DC Collectibles'
                        }
                  ],
                  DC: [
                        {
                              text: 'Terms Of Use'
                        },
                        {
                              text: 'Privacy policy (New)'
                        },
                        {
                              text: 'Ad Choices'
                        },
                        {
                              text: 'Advertising'
                        },
                        {
                              text: 'Jobs'
                        },
                        {
                              text: 'Subscriptions'
                        },
                        {
                              text: 'Talent Workshops'
                        },
                        {
                              text: 'CPSC Certificates'
                        },
                        {
                              text: 'Ratings'
                        },
                        {
                              text: 'Shop Help'
                        },
                        {
                              text: 'Contact Us'
                        },
                  ],
                  Sites: [
                        {
                              text: 'DC'
                        },
                        {
                              text: 'MAD Magazine'
                        },
                        {
                              text: 'DC Kids'
                        },
                        {
                              text: 'DC Universe'
                        },
                        {
                              text: 'DC Power Visa'
                        }
                  ],
                  Icons: [
                        {
                              url: 'footer-facebook.png',
                              name: 'facebook'
                        },
                        {
                              url: 'footer-periscope.png',
                              name: 'facebook'
                        },
                        {
                              url: 'footer-pinterest.png',
                              name: 'facebook'
                        },
                        {
                              url: 'footer-twitter.png',
                              name: 'facebook'
                        },
                        {
                              url: 'footer-youtube.png',
                              name: 'facebook'
                        },
                  ]
            }
      }
}
</script>
<template>
      <footer id="site_footer">
            <div class="contact_us">
                  <div class="my_container">
                        <div class="row">
                              <div class="col">
                                    <div class="row">
                                          <div class="col">
                                                <h3>dc comics</h3>
                                                <a href="#" v-for="item in DcComics">{{ item.text }}</a>

                                                <h3>shop</h3>
                                                <a href="#" v-for="item in Shop">{{ item.text }}</a>


                                          </div>
                                          <div class="col">
                                                <h3>DC</h3>
                                                <a href="#" v-for="item in DC">{{ item.text }}</a>

                                          </div>
                                          <div class="col">
                                                <h3>Sites</h3>

                                                <a href="#" v-for="item in Sites">{{ item.text }}</a>


                                          </div>
                                    </div>
                              </div>
                              <div class="col-7">
                                    <!-- <img src="../assets/img/dc-logo-bg.png" alt=""> -->
                              </div>
                        </div>
                  </div>

            </div>
            <div class="call_to_action">
                  <div class="my_container">
                        <button>
                              sign-up now!
                        </button>
                        <nav class="navbar">
                              <h3>follow us</h3>
                              <div>
                                    <a v-for="icon in Icons" href="#">
                                          <img :src="'../src/assets/img/' + icon.url" alt="">
                                    </a>
                              </div>
                        </nav>
                  </div>

            </div>
      </footer>
      <!-- /#site_footer -->
</template>
<style scoped>

</style>