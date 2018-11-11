<template>
  <ul>
    <li
      v-for="link in links"
      :key="link.title"
    >
      <a href="#">
        <i
          :class="link.iconClass"
          :title="link.title"
          class="aria-hidden"
        />
        <span class="sr-only">{{ link.title }}</span>
      </a>
    </li>
  </ul>
</template>

<script>
  export default {
    props: {
      links: {
        type: Array,
        default: () => []
      }
    }
  }
</script>

<style scoped>
  ul {
    display: flex;
    margin: 0;
    padding: 0;
    list-style: none;
  }

  a {
    display: block;
    margin-right: 8px;
    padding: 0;
    color: inherit;
    font-size: 16px;
    text-decoration: none;
    border: solid 1px currentColor;
    width: 2em;
    line-height: 2em;
    border-radius: 50%;
    text-align: center;
  }

  a:hover {
    background-color: rgba(0, 0, 0, 0.3);
  }
</style>
