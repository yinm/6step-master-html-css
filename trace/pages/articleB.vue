<template>
  <div>
    <Header />
    <Hero2 />
    <CardList2 />
    <Footer />
  </div>
</template>

<script>
  import CardList2 from '~/components/CardList2'
  import Footer from '~/components/Footer'
  import Header from '~/components/Header'
  import Hero2 from '~/components/Hero2'

  export default {
    components: {
      CardList2,
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
