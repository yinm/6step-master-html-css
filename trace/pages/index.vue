<template>
  <div>
    <Hero />
    <Concept />
    <Content />
    <ReversedContent />
  </div>
</template>

<script>
import Hero from '~/components/Hero.vue'
import Concept from '~/components/Concept.vue'
import Content from '~/components/Content.vue'
import ReversedContent from '~/components/ReversedContent.vue'

export default {
  components: {
    Hero,
    Concept,
    Content,
    ReversedContent
  }
}
</script>

<style>
body {
  margin: 0;
  font-family: 'メイリオ', 'Hiragino Kaku Gothic Pro', sans-serif;
}
</style>
