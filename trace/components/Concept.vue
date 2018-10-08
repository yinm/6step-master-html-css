<template>
  <section class="conB">
    <div class="container">
      <div class="text">
        <i class="far fa-chart-bar icon"/>
        <h2>ライフログって何？</h2>
        <p>日常のあれこれを記録していくライフログ。いろいろなものが見えてきます。</p>
        <a href="#">
          MORE...<i class="fas fa-chevron-right" />
        </a>
      </div>
    </div>
  </section>
</template>

<style scoped>
  .conB .text {
    text-align: center;
  }

  .conB .icon {
    margin-bottom: 20px;
    font-size: 40px;
    width: 2em;
    line-height: 2em;
    border-radius: 50%;
    text-align: center;
    background-color: var(--icon-bk-color);
    color: var(--icon-color);
  }

  .conB h2 {
    margin-top: 0;
    margin-bottom: 10px;
    font-size: 20px;
  }

  .conB p {
    margin-top: 0;
    margin-bottom: 20px;
    font-size: 14px;
    line-height: 1.8;
    opacity: 0.8;
  }

  .conB a {
    color: var(--main-color);
    text-decoration: none;
  }

  .conB a:hover {
    text-decoration: underline;
  }
</style>
