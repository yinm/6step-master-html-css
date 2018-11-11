<template>
  <footer>
    <div class="container">
      <div class="footA">
        <h2>LOGGER</h2>
        <p>
          〒000-0000 東京都中央区杉並3-3-3-403<br>
          <a href="#">http://logger.nett/</a>
        </p>

        <nav class="footD">
          <ul>
            <li>
              <a href="#">
                <i
                  class="aria-hidden fab fa-twitter icon"
                  title="Twitter"
                />
                <span class="sr-only">Twitter</span>
              </a>
            </li>
            <li>
              <a href="#">
                <i
                  class="aria-hidden fab fa-facebook-f icon"
                  title="facebook"
                />
                <span class="sr-only">Facebook</span>
              </a>
            </li>
            <li>
              <a href="#">
                <i
                  class="aria-hidden fab fa-google-plus-g icon"
                  title="Google Plus"
                />
                <span class="sr-only">Google Plus</span>
              </a>
            </li>
            <li>
              <a href="#">
                <i
                  class="aria-hidden fab fa-instagram icon"
                  title="Instagram"
                />
                <span class="sr-only">Instagram</span>
              </a>
            </li>
            <li>
              <a href="#">
                <i
                  class="aria-hidden fab fa-youtube icon"
                  title="YouTube"
                />
                <span class="sr-only">YouTube</span>
              </a>
            </li>
          </ul>
        </nav>
      </div>

      <nav class="footB">
        <footer-content :links="aboutLinks">ABOUT</footer-content>
        <footer-content :links="supportLinks">SUPPORT</footer-content>
        <footer-content :links="contentsLinks">CONTENTS</footer-content>
      </nav>

      <div class="footC">
        © LOGGER corp. All rights reserved.
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

  .footC {
    text-align: center;
    font-family: 'Montserrat', sans-serif;
    font-size: 12px;
  }

  .footD ul {
    display: flex;
    margin-top: 20px;
    padding: 0;
    list-style: none;
  }

  .footD li {
    margin-right: 7px;
  }

  .icon {
    border: solid 1px currentColor;
    border-radius: 50%;
    font-size: 15px;
    width: 2.2em;
    line-height: 2.2em;
    text-align: center;
  }

  .icon:hover {
    background-color: rgba(0, 0, 0, 0.3);
  }


  @media (min-width: 768px) {
    .container {
      display: flex;
      flex-wrap: wrap;
      max-width: var(--large-width);
      margin-left: auto;
      margin-right: auto;
    }

    .footA {
      flex: 0 0 40%;
    }

    .footB {
      display: flex;
      flex: 0 0 60%;
    }

    .footC {
      flex: 0 0 100%;
    }

    .footB div:not(:first-child) {
      margin-left: 40px;
    }
  }
</style>
