<template>
  <div>
    <logger-header />
    <Hero />
    <Concepts />
    <Content />
    <ReversedContent />
    <Footer />
  </div>
</template>

<script>
  import Hero from '~/components/Hero'
  import Concepts from '~/components/Concepts'
  import Content from '~/components/Content'
  import Footer from '~/components/Footer'
  import LoggerHeader from '~/components/LoggerHeader'
  import ReversedContent from '~/components/ReversedContent'

  export default {
    components: {
      Hero,
      Concepts,
      Content,
      Footer,
      LoggerHeader,
      ReversedContent
    }
  }
</script>

<style>
body {
  margin: 0;
  font-family: 'メイリオ', 'Hiragino Kaku Gothic Pro', sans-serif;
}

.sr-only {
  position: absolute;
  width: 1px;
  height: 1px;
  padding: 0;
  margin: -1px;
  overflow: hidden;
  clip: rect(0, 0, 0, 0);
  border: 0;
}
</style>
