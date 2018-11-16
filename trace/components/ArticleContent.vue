<template>
  <article class="post">
    <div class="container">
      <h1>ライフログのはじめ方</h1>
      <img
        src="/life.jpg"
        alt="eye catch"
      >
      <p>日常の生活を記録し、データとして残していく「ライフログ」。ブログで日記を書くことや、毎日食べたものを写真に撮って残していくといったことも、ライフログの１つです。記録をサポートしてくれるオンラインサービスやアプリもたくさんあります。</p>
      <p>手動で記録するのは面倒で…という場合も心配ありません。スマーフォトンやウェアラブルデバイスを利用すると、位置情報や睡眠時間などは自動的に記録することができます。体重計などの測定機器もクラウド化が進んでいますので、さまざまなデータが自動的に記録され、簡単に管理できる時代になっているのです。</p>
    </div>
  </article>
</template>

<style scoped>
.container {
  max-width: var(--middle-width);
  margin-left: auto;
  margin-right: auto;
  padding: 30px 10px;
}

h1 {
  font-size: 2.25rem;
  padding-left: 0.5rem;
  border-left: solid 0.875rem var(--accent-color);
}

img {
  max-width: 100%;
}

p {
  font-size: 1.125rem;
  line-height: 2;
}

@media (max-width: 767px) {
  :root {
    font-size: 14px;
  }
}

@media (max-width: 600px) {
  :root {
    font-size: 12px;
  }
}
</style>
