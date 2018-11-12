<template>
  <header>
    <div class="container">
      <a
        href="index.html"
        class="headA"
      >
        LOGGER
      </a>
    </div>
  </header>
</template>

<style scoped>
header {
  position: absolute;
  top: 0;
  left: 0;
  z-index: 100;
  width: 100%;
  background-color: rgba(255, 255, 255, 0.9);
}

.headA {
  display: inline-block;
  line-height: 70px;
  padding-left: 20px;
  padding-right: 20px;
  background-color: var(--main-color);
  color: var(--text-bright-color);
  font-family: 'Montserrat', sans-serif;
  font-size: 24px;
  text-decoration: none;
}
</style>
