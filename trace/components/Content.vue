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
  .conC {
    background-color: var(--main-color);
    color: var(--text-bright-color);
  }

  .conC h2 {
    margin-top: 0;
    margin-bottom: 10px;
    font-size: 20px;
  }

  .conC p {
    margin-top: 0;
    margin-bottom: 20px;
    font-size: 14px;
    line-height: 1.8;
    opacity: 0.8;
  }

  .conC a {
    display: inline-block;
    margin-top: 20px;
    padding: 10px 30px;
    border: solid 3px currentColor;
    border-radius: 6px;
    background-color: var(--accent-color);
    color: var(--text-bright-color);
    font-size: 14px;
    text-decoration: none;
  }

  .conC a:hover {
    background-image: linear-gradient(
      rgba(255, 255, 255, 0.2),
      rgba(255, 255, 255, 0.2)
    );
  }

  .conC .photo {
    min-height: 200px;
    background-image: url("/note.jpg");
    background-position: center;
    background-size: cover;
  }

  .conC .text {
    padding: 20px;
  }

  @media (min-width: 768px) {
    .conC .container {
      display: flex;
      max-width: var(--large-width);
      margin-left: auto;
      margin-right: auto;
    }

    .conC .photo {
      flex: 3;
    }

    .conC .text {
      flex: 2;
      padding: 50px;
    }
  }
</style>
