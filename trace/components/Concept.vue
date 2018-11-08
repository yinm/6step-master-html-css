<template>
  <section class="conB">
    <div class="container">
      <i class="far fa-chart-bar icon-mask" />
      <div class="text">
        <h2>ライフログって何？</h2>
        <p>日常のあれこれを記録していくライフログ。いろいろなものが見えてきます。</p>
        <a href="#">
          MORE...
          <i class="fas fa-chevron-right" />
        </a>
      </div>
    </div>
  </section>
</template>

<style scoped>
  .container {
    text-align: center;
  }

  .icon-mask {
    margin-bottom: 20px;
    font-size: 40px;
    width: 2em;
    line-height: 2em;
    border-radius: 50%;
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
</style>
