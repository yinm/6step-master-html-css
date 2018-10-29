<template>
  <div>
    <Header />
    <Hero2 />
    <Footer />
  </div>
</template>

<script>
  import Footer from '~/components/Footer'
  import Header from '~/components/Header'
  import Hero2 from '~/components/Hero2'

  export default {
    components: {
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
