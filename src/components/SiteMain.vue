<script>
export default {
      name: 'SiteMain',
      data() {
            return {
                  icons: [
                        {
                              image: 'buy-comics-digital-comics.png',
                              text: 'Digital Comics'
                        },
                        {
                              image: 'buy-comics-merchandise.png',
                              text: 'DC Merchandise'
                        },
                        {
                              image: 'buy-comics-subscriptions.png',
                              text: 'Subscriction'
                        },
                        {
                              image: 'buy-comics-shop-locator.png',
                              text: 'Comics shop locator'
                        },
                        {
                              image: 'buy-dc-power-visa.svg',
                              text: 'DC power visa'
                        }
                  ]
            }
      }
}
</script>
<template>
      <main id="site_main">
            <div class="jumbotron">
                  <h1> --> Content Goes Here </h1>
            </div>
            <div class="my-container">
                  <div class="row">
                        <div class="col" v-for="icon in icons">
                              <img :src="'./src/assets/img/' + icon.image" alt="">
                              <h3>{{ icon.text }}</h3>
                        </div>
                  </div>
            </div>
            <!-- /.jumbotron -->
      </main>
</template>
<style>

</style>