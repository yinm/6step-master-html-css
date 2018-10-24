<template>
  <article class="post">
    <div class="container">
      <h1>ライフログのはじめ方</h1>
      <div class="photo" />
      <p class="first">日常の生活を記録し、データとして残していく「ライフログ」。ブログで日記を書くことや、毎日食べたものを写真に撮って残していくといったことも、ライフログの１つです。記録をサポートしてくれるオンラインサービスやアプリもたくさんあります。</p>
      <p>手動で記録するのは面倒で…という場合も心配ありません。スマーフォトンやウェアラブルデバイスを利用すると、位置情報や睡眠時間などは自動的に記録することができます。体重計などの測定機器もクラウド化が進んでいますので、さまざまなデータが自動的に記録され、簡単に管理できる時代になっているのです。</p>
    </div>
  </article>
</template>

<style scoped>
  .container {
    padding: 30px 10px;
    max-width: var(--middle-width);
    margin-left: auto;
    margin-right: auto;
  }

  h1 {
    font-size: 36px;
    border-left: solid 14px var(--accent-color);
    padding-left: 9px;
  }

  p {
    font-size: 18px;
    line-height: 2;
  }

  .first {
    margin-top: 25px;
  }

  .photo {
    min-height: 530px;
    width: 100%;
    background-image: url("/life.jpg");
    background-position: center;
    background-size: cover;
  }

  @media (max-width: 800px) {
    h1 {
      font-size: 32px;
      border-left-width: 12px;
      padding-left: 8px;
    }

    .photo {
      min-height: 410px;
    }
  }

  @media (max-width: 600px) {
    h1 {
      font-size: 28px;
      border-left-width: 11px;
      padding-left: 7px;
    }

    .photo {
      min-height: 85px;
    }
  }
</style>
