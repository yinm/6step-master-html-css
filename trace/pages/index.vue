<template>
  <div>
    <Hero />
    <Concepts />
  </div>
</template>

<script>
  import Hero from '~/components/Hero'
  import Concepts from '~/components/Concepts'

  export default {
    components: {
      Hero,
      Concepts
    }
  }
</script>

<style>
  body {
    margin: 0;
    font-family: 'メイリオ', 'Hiragino Kaku Gothic Pro', sans-serif;
  }
</style>
