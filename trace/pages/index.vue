<template>
  <div>
    <Hero />
    <Concepts />
    <Content />
  </div>
</template>

<script>
  import Hero from '~/components/Hero'
  import Concepts from '~/components/Concepts'
  import Content from '~/components/Content'

  export default {
    components: {
      Hero,
      Concepts,
      Content
    }
  }
</script>

<style>
  body {
    margin: 0;
    font-family: 'メイリオ', 'Hiragino Kaku Gothic Pro', sans-serif;
  }
</style>
