<template>
  <section class="listA">
    <h1 class="sr-only">RECENT POSTS</h1>
    <div class="container">
      <Card :thumb-src="'/p01.jpg'">
        <h2 slot="title">黄色い花を飾ってみた</h2>
        <p slot="description">黄色い花を部屋に飾るといいことがあるかもしれません。その理由は…</p>
      </Card>
      <Card :thumb-src="'/p02.jpg'">
        <h2 slot="title">野菜の成長記録</h2>
        <p slot="description">野菜たちはすくすく成長しています。おもしろいので試しに記録を残してみます。</p>
      </Card>
      <Card :thumb-src="'/p03.jpg'">
        <h2 slot="title">野苺のおいしい食べ方</h2>
        <p slot="description">野苺をたくさんもらって困ってももう大丈夫。おいしく食べきることができます。</p>
      </Card>
      <Card :thumb-src="'/p04.jpg'">
        <h2 slot="title">音の響き方</h2>
        <p slot="description">音の響き方で物事の印象が変わる。そんなお話です。</p>
      </Card>
      <Card :thumb-src="'/p05.jpg'">
        <h2 slot="title">かわいい模様</h2>
        <p slot="description">あちこちで見かけるかわいい模様の秘密を探ってきました。</p>
      </Card>
      <Card :thumb-src="'/p06.jpg'">
        <h2 slot="title">砂糖と水分の甘い関係</h2>
        <p slot="description">水は生き物にとって欠かせないものです。そして、甘いものも。</p>
      </Card>
      <Card :thumb-src="'/p07.jpg'">
        <h2 slot="title">ライフログのはじめ方</h2>
        <p slot="description">日常の生活を記録し、データとして残していく「ライフログ」。</p>
      </Card>
      <Card :thumb-src="'/p08.jpg'">
        <h2 slot="title">管理はおまかせ</h2>
        <p slot="description">面倒な設定やデータ管理、アプリとの連携などは全部おまかせ。</p>
      </Card>
      <Card :thumb-src="'/p09.jpg'">
        <h2 slot="title">快適ロングステイ</h2>
        <p slot="description">快適に過ごすポイントを抑えておけばロングステイも問題なしです。</p>
      </Card>
      <Card :thumb-src="'/p10.jpg'">
        <h2 slot="title">空を飛んでみた</h2>
        <p slot="description">ちょっと空を飛んできました。眺めが良くて最高です。</p>
      </Card>
      <Card :thumb-src="'/p11.jpg'">
        <h2 slot="title">サラダの記録</h2>
        <p slot="description">世の中にはバリエーション豊かなサラダがたくさんあります。</p>
      </Card>
      <Card :thumb-src="'/p12.jpg'">
        <h2 slot="title">こまめな連絡が大事</h2>
        <p slot="description">何事もこまめな連絡が大事です。これはそんなお話です。</p>
      </Card>
    </div>
  </section>
</template>

<script>
  import Card from './Card3'

  export default {
    components: {
      Card: Card
    }
  }
</script>

<style scoped>
  h1 {
    text-align: center;
  }

  .container {
    display: flex;
    flex-wrap: wrap;
    max-width: var(--extra-large-width);
  }
</style>
