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
    flex: 1 1 384px;
    display: flex;
  }

  a {
    flex: 1;
    margin: 10px;
    display: flex;
    border: solid 1px var(--gray-color);
    color: inherit;
    text-decoration: none;
  }

  a:hover {
    opacity: 0.8;
  }

  .photo {
    flex: 2;
    min-height: 0;
    background-position: center;
    background-size: cover;
  }

  .text {
    flex: 3;
    margin: 10px;
  }

  h2 {
    font-size: 18px;
  }

  p {
    font-size: 14px;
    opacity: 0.8;
  }

  @media (max-width: 384px) {
    .photo {
      flex: 1;
    }

    p {
      display: none;
    }
  }
</style>
