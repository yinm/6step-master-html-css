<template>
  <div>
    <h3><slot /></h3>
    <ul>
      <li
        v-for="link in links"
        :key="link.name"
      >
        <a :href="link.anchor">{{ link.name }}</a>
      </li>
    </ul>
  </div>
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
  div {
    margin-bottom: 20px;
  }

  h3 {
    margin-top: 0;
    margin-bottom: 10px;
    border-bottom: solid 1px currentColor;
    font-size: 14px;
  }

  ul {
    margin: 0;
    padding: 0;
    list-style: none;
  }

  a {
    display: block;
    padding: 5px;
    color: inherit;
    font-size: 12px;
    text-decoration: none;
  }

  a:hover {
    background-color: rgba(0, 0, 0, 0.3);
  }

  @media (min-width: 768px) {
    div {
      flex: 1;
    }
  }
</style>
