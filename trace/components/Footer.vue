<template>
  <footer>
    <div class="container">
      <div class="footA">
        <h2>LOGGER</h2>
        <p>
          〒000-0000 東京都中央区杉並3-3-3-403<br>
          <a href="#">http://logger.nett/</a>
        </p>
      </div>

      <nav class="footB">
        <footer-content :links="aboutLinks">ABOUT</footer-content>
        <footer-content :links="supportLinks">SUPPORT</footer-content>
        <footer-content :links="contentsLinks">CONTENTS</footer-content>
      </nav>

      <div class="footC">
        <p>© LOGGER corp. All rights reserved.</p>
      </div>
    </div>
  </footer>
</template>

<script>
  import FooterContent from './FooterContent'

  export default {
    components: {
      FooterContent
    },

    data() {
      return {
        aboutLinks: [
          {
            name: '設立',
            anchor: '#'
          },
          {
            name: '所在地',
            anchor: '#'
          },
          {
            name: '地図',
            anchor: '#'
          },
          {
            name: 'スタッフ',
            anchor: '#'
          }
        ],
        supportLinks: [
          {
            name: 'ダウンロード',
            anchor: '#'
          },
          {
            name: 'マニュアル',
            anchor: '#'
          },
          {
            name: 'よくある質問',
            anchor: '#'
          },
          {
            name: 'お問い合わせ',
            anchor: '#'
          }
        ],
        contentsLinks: [
          {
            name: 'お知らせ',
            anchor: '#'
          },
          {
            name: 'ビジネス',
            anchor: '#'
          },
          {
            name: 'プロフィール',
            anchor: '#'
          },
          {
            name: '開発者',
            anchor: '#'
          },
          {
            name: 'ブログ',
            anchor: '#'
          }
        ]
      }
    }
  }
</script>

<style scoped>
  footer {
    color: var(--text-bright-color);
    background-color: var(--dark-main-color);
  }

  .container {
    padding: 40px 20px;
  }

  .footA {
    margin-bottom: 30px;
  }

  h2 {
    margin-top: 0;
    margin-bottom: 10px;
    font-family: 'Montserrat', sans-serif;
    font-size: 30px;
    letter-spacing: 0.2em;
  }

  p {
    margin: 0;
    font-size: 14px;
  }

  a {
    color: inherit;
    font-size: 14px;
    text-decoration: none;
  }

  .footC p {
    text-align: center;
    font-family: 'Montserrat', sans-serif;
    font-size: 12px;
  }

  @media (min-width: 768px) {
    .footB {
      display: flex;
    }

    .footB div:not(:first-child) {
      margin-left: 40px;
    }
  }
</style>
