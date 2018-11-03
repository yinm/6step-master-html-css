<template>
  <div>
    <Header />
    <Hero2 />
    <CardList3 />
    <Footer />
  </div>
</template>

<script>
  import CardList3 from '~/components/CardList3'
  import Footer from '~/components/Footer'
  import Header from '~/components/Header'
  import Hero2 from '~/components/Hero2'

  export default {
    components: {
      CardList3,
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
