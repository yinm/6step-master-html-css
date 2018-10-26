<template>
  <div>
    <Header :is-hero-image="false" />
    <About />
    <Footer />
  </div>
</template>

<script>
import About from '~/components/About'
import Header from '~/components/Header'
import Footer from '~/components/Footer'

export default {
  components: {
    About,
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
