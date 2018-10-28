<template>
  <div>
    <Header :is-hero-image="false" />
    <Contact />
    <Footer />
  </div>
</template>

<script>
import Contact from '~/components/Contact'
import Footer from '~/components/Footer'
import Header from '~/components/Header'

export default {
  components: {
    Contact,
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
