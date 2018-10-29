<template>
  <article>
    <a href="#">
      <div
        :style="{ backgroundImage: 'url(' + thumbSrc + ')' }"
        class="photo"
      />
      <div class="text">
        <slot name="title" />
        <slot name="description" />
      </div>
    </a>
  </article>
</template>

<script>
  export default {
    props: {
      thumbSrc: {
        type: String,
        default: ''
      }
    }
  }
</script>

<style scoped>
  article {
    flex: 1 1 300px;
  }

  a {
    margin: 10px;
    display: block;
    border: solid 1px var(--gray-color);
    color: inherit;
    text-decoration: none;
  }

  a:hover {
    opacity: 0.8;
  }

  .photo {
    min-height: 150px;
    background-position: center;
    background-size: cover;
  }

  .text {
    margin: 10px;
  }

  h2 {
    font-size: 18px;
  }

  p {
    font-size: 14px;
    opacity: 0.8;
  }
</style>
