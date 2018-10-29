<template>
  <a href="#">
    <div class="photo" />
    <div class="text-container">
      <h2>黄色い花を飾ってみた</h2>
      <p>黄色い花を部屋に飾るといいことがあるかもしれません。その理由は…</p>
    </div>
  </a>
</template>

<style scoped>
  a {
    display: block;
    margin: 10px;
    border: solid 1px var(--gray-color);
    text-decoration: none;
    color: inherit;
  }

  a:hover {
    opacity: 0.8;
  }

  .photo {
    height: 150px;
    width: 100%;
    background-image: url('/p01.jpg');
    background-position: center;
    background-size: cover;
  }

  .text-container {
    padding-left: 10px;
    padding-right: 10px;
  }

  h2 {
    font-size: 18px;
  }

  p {
    font-size: 14px;
    opacity: 0.7;
  }
</style>
