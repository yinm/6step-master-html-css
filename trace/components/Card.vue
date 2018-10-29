<template>
  <article>
    <a href="#">
      <div
        :style="{ backgroundImage: 'url(' + thumbSrc + ')' }"
        class="photo"
      />
      <div class="text">
        <h2>黄色い花を飾ってみた</h2>
        <p>黄色い花を部屋に飾るといいことがあるかもしれません。その理由は…</p>
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
