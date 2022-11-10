<script>
export default {
      name: 'SiteHeader',
      data() {
            return {
                  menu: [
                        {
                              text: 'characters',
                              href: '#'
                        },
                        {
                              text: 'comics',
                              href: '#'
                        },
                        {
                              text: 'movies',
                              href: '#'
                        },
                        {
                              text: 'tv',
                              href: '#'
                        },
                        {
                              text: 'games',
                              href: '#'
                        },
                        {
                              text: 'collectibles',
                              href: '#'
                        },
                        {
                              text: 'videos',
                              href: '#'
                        },
                        {
                              text: 'fans',
                              href: '#'
                        },
                        {
                              text: 'news',
                              href: '#'
                        },
                        {
                              text: 'shop',
                              href: '#'
                        }
                  ]
            }
      }
}
</script>
<template>
      <header id="site_header">
            <div class="container">
                  <div class="logo">
                        <img src="../assets/img/dc-logo.png" alt="">
                  </div>
                  <nav class="navbar">
                        <a :href="item.href" v-for="item in menu" :class="item.text === 'comics' ? 'active' : ''">
                              {{ item.text }}
                        </a>
                  </nav>
                  <!-- /.navbar -->
            </div>
      </header>
</template>
<style>

</style>