<template>
  <article>
    <div class="container">
      <h1>LOGGERについて</h1>
      <p>LOGGERはライフログに関する情報の発信、アプリ開発、データの分析、ユーザーサポートを行うために設立された会社です。ライフログのサービスやデータを活用することで、日々の生活を楽しみ、よりよくしていくことを目指しています。</p>
      <p>近年はグローバルワールドネットワークとも提携し、国内のみならず、海外展開も含めて活動の場をひろげています。</p>
    </div>
    <about-history />
  </article>
</template>

<script>
import AboutHistory from './AboutHistory'

export default {
  components: {
    AboutHistory
  }
}
</script>

<style scoped>
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

.container {
  max-width: var(--middle-width);
  margin-left: auto;
  margin-right: auto;
  padding: 30px 10px;
}

h1 {
  margin-top: 30px;
  margin-bottom: 30px;
  border-left: solid 0.75rem var(--accent-color);
  padding-left: 0.5rem;
  font-size: 2rem;
}

p {
  font-size: 1rem;
  line-height: 2;
}
</style>

