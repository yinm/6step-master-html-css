<template>
  <div>
    <Hero />
    <Concept />
  </div>
</template>

<script>
import Hero from '~/components/Hero.vue'
import Concept from '~/components/Concept.vue'

export default {
  components: {
    Hero,
    Concept
  }
}
</script>

<style>
body {
  margin: 0;
  font-family: 'メイリオ', 'Hiragino Kaku Gothic Pro', sans-serif;
}
</style>
