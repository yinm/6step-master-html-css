<template>
  <div>
    <Header />
    <Hero />
    <Concept />
    <Content />
    <ReversedContent />
    <Footer />
  </div>
</template>

<script>
import Hero from '~/components/Hero.vue'
import Concept from '~/components/Concept.vue'
import Content from '~/components/Content.vue'
import Header from '~/components/Header.vue'
import ReversedContent from '~/components/ReversedContent.vue'
import Footer from '~/components/Footer.vue'

export default {
  components: {
    Hero,
    Concept,
    Content,
    Header,
    ReversedContent,
    Footer
  }
}
</script>

<style>
body {
  margin: 0;
  font-family: 'メイリオ', 'Hiragino Kaku Gothic Pro', sans-serif;
}
</style>
