<template>
  <div class="text">
    <i
      :class="iconClass"
      class="icon"
    />
    <slot name="title" />
    <slot name="description" />
    <a href="#">
      MORE...
      <i class="fas fa-chevron-right" />
    </a>
  </div>
</template>

<script>
  export default {
    props: {
      iconClass: {
        type: String,
        default: 'far fa-chart-bar'
      }
    },
  }
</script>

<style scoped>
  .text {
    padding-left: 20px;
    padding-right: 20px;
    padding-bottom: 60px;
    text-align: center;
  }

  .icon {
    display: inline-block;
    margin-bottom: 20px;
    font-size: 40px;
    width: 2em;
    line-height: 2em;
    border-radius: 50%;
    text-align: center;
    background-color: var(--icon-bk-color);
    color: var(--icon-color);
  }

  h2 {
    margin-top: 0;
    margin-bottom: 10px;
    font-size: 20px;
  }

  p {
    margin-top: 0;
    margin-bottom: 20px;
    font-size: 14px;
    line-height: 1.8;
    opacity: 0.8;
  }

  a {
    color: var(--main-color);
    text-decoration: none;
  }

  a:hover {
    text-decoration: underline;
  }

  @media (min-width: 768px) {
    .text {
      flex: 1;
    }
  }
</style>
