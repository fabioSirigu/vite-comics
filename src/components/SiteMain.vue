<script>
import IconSection from './IconSection.vue'
import ComicsCard from './ComicsCard.vue'
import Comics from './data/Comics.js'
export default {
      name: 'SiteMain',
      components: {
            IconSection,
            ComicsCard
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
            <div class="jumbotron">
                  <div class="container">
                        <div class="row">
                              <ComicsCard v-for="comic in comics" :url="comic.thumb" :title="comic.series" />

                        </div>
                  </div>
            </div>
            <IconSection />
            <!-- /.jumbotron -->
      </main>
</template>
<style>

</style>