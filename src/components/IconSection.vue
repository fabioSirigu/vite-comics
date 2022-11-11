<script>
export default {
      name: 'IconSection',
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

      },
      methods: {
            getImageUrl(name) {
                  return new URL(`../assets/img/${name}`, import.meta.url).href
            }
      }
}
</script>
<template>
      <div class="my-container">
            <div class="row">
                  <div class="col" v-for="icon in icons">
                        <img :src="getImageUrl(icon.image)" alt="">
                        <h3>{{ icon.text }}</h3>
                  </div>
            </div>
      </div>
</template>
<style scoped>

</style>