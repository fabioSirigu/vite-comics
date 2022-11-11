<script>
import IconSection from './IconSection.vue'
import ComicsCard from './ComicsCard.vue'
import BannerSection from './BannerSection.vue'
import Comics from './data/Comics.js'
export default {
      name: 'SiteMain',
      components: {
            IconSection,
            ComicsCard,
            BannerSection
      },
      data() {
            return {
                  comics: Comics
            }
      }

}
</script>
<template>
      <main id="site_main">
            <BannerSection />

            <div class="jumbotron">
                  <div class="container">
                        <div class="row">
                              <ComicsCard v-for="comic in comics" :url="comic.thumb" :title="comic.series" />
                        </div>
                  </div>
                  <div class="load_more">
                        <h3>Load More</h3>
                  </div>
            </div>
            <IconSection />
            <!-- /.jumbotron -->
      </main>
</template>
<style>

</style>