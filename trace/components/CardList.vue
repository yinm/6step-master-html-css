<template>
  <section class="listA">
    <div class="container">
      <Card :thumb-src="'/p01.jpg'" />
    </div>
  </section>
</template>

<script>
  import Card from './Card'

  export default {
    components: {
      Card
    }
  }
</script>

<style scoped>
</style>
