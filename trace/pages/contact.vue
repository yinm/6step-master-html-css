<template>
  <div>
    <logger-header :is-no-hero-image="true" />
    <contact-view />
    <Footer />
  </div>
</template>

<script>
import ContactView from '~/components/ContactView'
import Footer from '~/components/Footer'
import LoggerHeader from '~/components/LoggerHeader'

export default {
  components: {
    ContactView,
    Footer,
    LoggerHeader
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
