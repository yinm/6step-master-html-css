<template>
  <div>
    <Hero />
    <Concepts />
    <Content />
    <ReversedContent />
  </div>
</template>

<script>
  import Hero from '~/components/Hero'
  import Concepts from '~/components/Concepts'
  import Content from '~/components/Content'
  import ReversedContent from '~/components/ReversedContent'

  export default {
    components: {
      Hero,
      Concepts,
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
