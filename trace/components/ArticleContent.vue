<template>
  <article class="post">
    <div class="container">
      <div class="bread">
        <ol>
          <li>
            <a href="#">トップ</a>
          </li>
          <li>
            <a href="#">記事一覧</a>
          </li>
        </ol>
      </div>

      <h1>ライフログのはじめ方</h1>
      <img
        src="/life.jpg"
        alt=""
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

@media (max-width: 599px) {
  :root {
    font-size: 14px;
  }
}

@media (min-width: 600px) and (max-width: 799px) {
  :root {
    font-size: 16px;
  }
}

@media (min-width: 800px) {
  :root {
    font-size: 18px;
  }
}

body {
  font-size: 16px;
}

h1 {
  padding-left: 0.5rem;
  border-left: solid 0.75rem var(--accent-color);
  font-size: 2rem;
}

p {
  font-size: 1rem;
  line-height: 2;
}

img {
  max-width: 100%;
}

.bread ol {
  display: flex;
  margin: 0;
  padding: 0;
  list-style: none;
}

.bread a {
  display: block;
  padding: 5px;
  color: inherit;
  font-size: 0.875rem;
  text-decoration: none;
}

.bread a:hover {
  background-color: rgba(0, 0, 0, 0.3);
}

.bread a::after {
  margin-left: 10px;
  content: '\f054';
  font-family: 'Font Awesome 5 Free';
  opacity: 0.3;
}
</style>
