<template>
  <div>
    <Header :isHeroImage="false" />
    <Article />
    <Footer />
  </div>
</template>

<script>
import Article from '~/components/Article.vue'
import Footer from '~/components/Footer.vue'
import Header from '~/components/Header.vue'

export default {
  components: {
    Article,
    Footer,
    Header,
  }
}
</script>

<style>
body {
  margin: 0;
  font-family: 'メイリオ', 'Hiragino Kaku Gothic Pro', sans-serif;
}
</style>
