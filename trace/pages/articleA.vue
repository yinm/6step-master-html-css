<template>
  <div>
    <Header />
    <Hero2 />
    <Card />
    <Footer />
  </div>
</template>

<script>
  import Card from '~/components/Card'
  import Footer from '~/components/Footer'
  import Header from '~/components/Header'
  import Hero2 from '~/components/Hero2'

  export default {
    components: {
      Card,
      Footer,
      Header,
      Hero2,
    }
  }
</script>

<style>
body {
  margin: 0;
  font-family: 'メイリオ', 'Hiragino Kaku Gothic Pro', sans-serif;
}
</style>
