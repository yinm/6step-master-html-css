<template>
  <main>
    <div class="container">
      <h2 class="about-title">LOGGERについて</h2>
      <p class="about-description">LOGGERはライフログに関する情報の発信、アプリ開発、データの分析、ユーザーサポートを行うために設立された会社です。ライフログのサービスやデータを活用することで、日々の生活を楽しみ、よりよくしていくことを目指しています。</p>
      <p class="about-description">近年はグローバルワールドネットワークとも提携し、国内のみならず、海外展開も含めて活動の場をひろげています。</p>
    </div>
    <ContentForAbout />
  </main>
</template>

<script>
import ContentForAbout from '~/components/ContentForAbout'

export default {
  components: {
    ContentForAbout,
  }
}
</script>

<style scoped>
  .container {
    max-width: var(--middle-width);
    margin-left: auto;
    margin-right: auto;
    padding: 30px 10px;
  }

  body {
    font-size: 16px;
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

  .about-title {
    padding-left: 0.5rem;
    border-left: solid 0.75rem var(--accent-color);
    font-size: 2rem;
  }

  .about-description {
    font-size: 1rem;
    line-height: 2;
  }
</style>
