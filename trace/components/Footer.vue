<template>
  <footer>
    <div class="container">

      <div class="footA">
        <h2>LOGGER</h2>
        <p>
          〒000-0000 東京都中央区杉並3-3-3-403<br>
          <a href="#">http://logger.nett/</a>
        </p>

        <ul>
          <li><i class="fab fa-twitter" /></li>
          <li><i class="fab fa-facebook-f" /></li>
          <li><i class="fab fa-google-plus-g" /></li>
          <li><i class="fab fa-instagram" /></li>
          <li><i class="fab fa-youtube" /></li>
        </ul>
      </div>

      <nav class="footB">
        <div>
          <h3>ABOUT</h3>
          <ul>
            <li><a href="#">設立</a></li>
            <li><a href="#">所在地</a></li>
            <li><a href="#">地図</a></li>
            <li><a href="#">スタッフ</a></li>
          </ul>
        </div>

        <div>
          <h3>SUPPORT</h3>
          <ul>
            <li><a href="#">ダウンロード</a></li>
            <li><a href="#">マニュアル</a></li>
            <li><a href="#">よくある質問</a></li>
            <li><a href="#">お問い合わせ</a></li>
          </ul>
        </div>

        <div>
          <h3>CONTENTS</h3>
          <ul>
            <li><a href="#">お知らせ</a></li>
            <li><a href="#">ビジネス</a></li>
            <li><a href="#">プロフィール</a></li>
            <li><a href="#">開発者</a></li>
            <li><a href="#">ブログ</a></li>
          </ul>
        </div>
      </nav>

      <div class="footC">
        © LOGGER corp. All rights reserved.
      </div>

    </div>
  </footer>
</template>

<style scoped>
  @import url('https://fonts.googleapis.com/css?family=Montserrat');

  footer {
    color: var(--text-bright-color);
    background-color: var(--dark-main-color);
  }

  footer .container {
    padding: 40px 20px;
  }

  .footA {
    margin-bottom: 30px;
  }

  .footA h2 {
    margin-top: 0;
    margin-bottom: 10px;
    font-family: 'Montserrat', sans-serif;
    font-size: 30px;
    letter-spacing: 0.2em;
  }

  .footA p {
    margin-top: 0;
    margin-bottom: 0;
    font-size: 14px;
  }

  .footA a {
    color: inherit;
    text-decoration: none;
  }

  .footB div {
    margin-bottom: 20px;
  }

  .footB h3 {
    margin-top: 0;
    margin-bottom: 10px;
    border-bottom: solid 1px currentColor;
    font-size: 14px;
  }

  .footB ul {
    margin: 0;
    padding: 0;
    list-style: none;
  }

  .footB a {
    display: block;
    padding: 5px;
    color: inherit;
    font-size: 12px;
    text-decoration: none;
  }

  .footB a:hover {
    background-color: rgba(0, 0, 0, 0.3);
  }

  .footC {
    font-size: 12px;
    text-align: center;
    font-family: 'Montserrat', sans-serif;
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

    .footB div {
      flex: 1;
    }

    .footB div:not(:first-child) {
      margin-left: 40px;
    }
  }
</style>
