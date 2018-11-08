<template>
  <section class="conB">
    <div class="container">
      <Concept icon-class="far fa-chart-bar">
        <h2 slot="title">ライフログって何？</h2>
        <p slot="description">日常のあれこれを記録していくライフログ。いろいろなものが見えてきます。</p>
      </Concept>
      <Concept icon-class="fas fa-cogs icon">
        <h2 slot="title">必要なのはスマホだけ</h2>
        <p slot="description">ライフログを始めるのに必要なのはスマホだけ。いつでもスタートできます。</p>
      </Concept>
      <Concept icon-class="fas fa-rocket icon">
        <h2 slot="title">SNSとの連携も簡単</h2>
        <p slot="description">TwitterやFacebookといったSNSと連携して、簡単にログを共有することができます。</p>
      </Concept>
    </div>
  </section>
</template>

<script>
  import Concept from './Concept'

  export default {
    components: {
      Concept
    }
  }
</script>

<style scoped>
  .container {
    padding-top: 80px;
    padding-bottom: 20px;
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
    padding-left: 20px;
    padding-right: 20px;
    padding-bottom: 60px;
    text-align: center;
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
      max-width: var(--large-width);
      margin-left: auto;
      margin-right: auto;
    }

    .text {
      flex: 1;
    }
  }
</style>
