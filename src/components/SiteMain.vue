<script>
export default {
      name: 'SiteMain',
      data() {
            return {
                  icons: [
                        {
                              image: '../assets/img/buy-comics-digital-comics.png',
                              text: 'Digital comics'
                        },
                        {
                              image: '',
                              text: 'Digital comics'
                        },
                        {
                              image: '',
                              text: 'Digital comics'
                        },
                        {
                              image: '',
                              text: 'Digital comics'
                        },
                        {
                              image: '',
                              text: 'Digital comics'
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
                              <img :src="icon.image" alt="">
                              <h3>{{ icon.text }}</h3>
                        </div>
                  </div>
            </div>
            <!-- /.jumbotron -->
      </main>
</template>
<style>

</style>