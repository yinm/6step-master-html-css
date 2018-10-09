<template>
  <section class="conC">
    <div class="container">
      <div class="img" />
      <div class="text">
        <h2>面倒な設定やデータの管理は全部おまかせ</h2>
        <p>ライフログでつまずきがちな面倒な設定やデータ管理の煩わしさはありません。他のログアプリとの連携もワンクリックで完了です。</p>
      </div>
      <a href="#">
        詳しい設定方法を確認する
        <i class="fas fa-chevron-right" />
      </a>
    </div>
  </section>
</template>

<style scoped>
  .conC {
    background-color: var(--main-color);
    color: var(--text-bright-color);
  }

  .conC .img {
    height: 200px;
    width: 100%;
    background-image: url("/note.jpg");
    background-size: cover;
    background-position: center;
  }

  .conC .text {
    padding-bottom: 42px;
  }

  .conC .text h2 {
    margin-top: 0;
    margin-bottom: 12px;
    font-size: 20px;
  }

  .conC .text p {
    margin: 0;
    font-size: 14px;
    opacity: 0.8;
  }

  .conC a {
    display: inline-block;
    border: 3px solid var(--text-bright-color);
    border-radius: 6px;
    padding: 10px 30px;
    background-color: var(--accent-color);
    color: var(--text-bright-color);
    font-size: 14px;
    text-decoration: none;
  }

  .conC a:hover {
    background-image: linear-gradient(
      rgba(255, 255, 255, 0.3),
      rgba(255, 255, 255, 0.3)
    );
  }
</style>
