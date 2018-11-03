<template>
  <article>
    <a
      :style="{ backgroundImage: 'linear-gradient(rgba(0, 0, 0, 0.4), rgba(0, 0, 0, 0.4)), url(' + thumbSrc + ')' }"
      class="photo"
      href="#"
    >
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
    margin-top: 3px;
    display: flex;
  }

  a {
    flex: 1;
    display: flex;
    align-items: flex-end;
    margin: 2px;
    border: solid 1px var(--gray-color);
    min-height: 250px;
    color: #fff;
    text-decoration: none;
  }

  a:hover {
    opacity: 0.8;
  }

  .photo {
    background-position: center;
    background-size: cover;
  }

  .text {
    margin-left: 10px;
    margin-right: 10px;
  }

  h2 {
    margin: 0;
    font-size: 18px;
  }

  p {
    margin-top: 0;
    margin-bottom: 10px;
    font-size: 14px;
    opacity: 0.8;
  }
</style>
