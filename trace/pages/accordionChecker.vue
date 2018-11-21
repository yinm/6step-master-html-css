<template>
  <div>
    <menu-accordion>
      <div slot="title">アコーディオン1</div>
      <div slot="body">
        <p>アコーディオンの中身</p>
        <p>アコーディオンの中身</p>
        <p>アコーディオンの中身</p>
      </div>
    </menu-accordion>

    <menu-accordion>
      <div slot="title">アコーディオン2</div>
      <ul slot="body">
        <li>アコーディオンの中身</li>
        <li>アコーディオンの中身</li>
        <li>アコーディオンの中身</li>
      </ul>
    </menu-accordion>
  </div>
</template>

<script>
import MenuAccordion from '~/components/MenuAccordion'

export default {
  components: {
    MenuAccordion
  }
}
</script>

<style scoped>
</style>
