<template>
  <article>
    <a
      href="#"
    >
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
    flex: 1 1 250px;
    display: flex;
  }

  a {
    position: relative;
    flex: 1;
    margin: 2px;
    display: block;
    border: solid 1px var(--gray-color);
    background-color: #000;
    color: inherit;
    text-decoration: none;
  }

  a:hover {
    opacity: 0.8;
  }

  .photo {
    min-height: 250px;
    background-position: center;
    background-size: cover;
    opacity: 0.6;
  }

  .text {
    position: absolute;
    bottom: 0;
    left: 0;
    margin: 10px;
    color: var(--text-bright-color);
  }

  h2 {
    margin: 0;
    font-size: 18px;
  }

  p {
    margin: 0;
    font-size: 14px;
    opacity: 0.8;
  }

  @media (min-width: 1000px) {
    article {
      flex: 1 1 25%;
    }
  }
</style>
