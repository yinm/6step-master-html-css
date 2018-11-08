<template>
  <section class="conB">
    <div class="container">
      <div class="text">
        <i class="far fa-chart-bar icon" />
        <h2>ライフログって何？</h2>
        <p>日常のあれこれを記録していくライフログ。いろいろなものが見えてきます。</p>
        <a href="#">
          MORE...
          <i class="fas fa-chevron-right" />
        </a>
      </div>
      <div class="text">
        <i class="fas fa-cogs icon" />
        <h2>必要なのはスマホだけ</h2>
        <p>ライフログを始めるのに必要なのはスマホだけ。いつでもスタートできます。</p>
        <a href="#">
          MORE...
          <i class="fas fa-chevron-right" />
        </a>
      </div>
      <div class="text">
        <i class="fas fa-rocket icon" />
        <h2>SNSとの連携も簡単</h2>
        <p>TwitterやFacebookといったSNSと連携して、簡単にログを共有することができます。</p>
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
    padding: 80px 20px;
  }

  .icon {
    display: inline-block;
    margin-bottom: 20px;
    font-size: 40px;
    width: 2em;
    line-height: 2em;
    border-radius: 50%;
    text-align: center;
    background-color: var(--icon-bk-color);
    color: var(--icon-color);
  }

  .text {
    text-align: center;
  }

  .text:not(:last-child) {
    margin-bottom: 60px;
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

  @media (min-width: 768px) {
    .container {
      display: flex;
      margin: 0 auto;
      padding-bottom: 0;
      max-width: var(--large-width);
    }

    .text {
      flex: 1;
    }
  }
</style>
