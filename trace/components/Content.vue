<template>
  <section class="conC">
    <div class="container">
      <div class="photo" />
      <div class="text">
        <h2>面倒な設定やデータの管理は全部おまかせ</h2>
        <p>ライフログでつまずきがちな面倒な設定やデータ管理の煩わしさはありません。他のログアプリとの連携もワンクリックで完了です。</p>
        <a href="#">
          詳しい設定方法を確認する
          <i class="fas fa-chevron-right" />
        </a>
      </div>
    </div>
  </section>
</template>

<style scoped>
  .photo {
    height: 200px;
    width: 100%;
    background-image: url("/note.jpg");
    background-position: center;
    background-size: cover;
  }

  .text {
    background-color: var(--main-color);
    color: var(--text-bright-color);
  }

  h2 {
    margin-top: 0;
    margin-bottom: 10px;
    font-size: 20px;
  }

  p {
    margin-top: 0;
    margin-bottom: 40px;
    font-size: 14px;
    line-height: 1.8;
    opacity: 0.8;
  }

  a {
    display: inline-block;
    padding: 10px 30px;
    border: solid 3px currentColor;
    border-radius: 6px;
    background-color: var(--accent-color);
    text-decoration: none;
    color: inherit;
    font-size: 14px;
  }

  a:hover {
    background-image: linear-gradient(
      rgba(255, 255, 255, 0.2),
      rgba(255, 255, 255, 0.2)
    );
  }
</style>
