<template>
  <section class="conB">
    <div class="container">
      <i class="far fa-chart-bar chart"/>
      <div class="text">
        <h2>ライフログって何？</h2>
        <p>日常のあれこれを記録していくライフログ。いろいろなものが見えてきます。</p>
        <a href="#">
          MORE...<i class="fas fa-chevron-right chevron" />
        </a>
      </div>
    </div>
  </section>
</template>

<style scoped>
  .conB {
    text-align: center;
  }

  .conB .chart {
    margin-bottom: 20px;
    padding: 15px;
    border-radius: 50%;
    background-color: #ddd;
    font-size: 3rem;
    color: #fff;
  }

  .conB .chevron {
    margin-left: 5px;
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
