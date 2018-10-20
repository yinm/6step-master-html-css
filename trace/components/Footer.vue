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

      <div class="footB">
        <h3 class="list-title">ABOUT</h3>
        <ul>
          <li>
            <a href="#">設立</a>
          </li>
          <li>
            <a href="#">所在地</a>
          </li>
          <li>
            <a href="#">地図</a>
          </li>
          <li>
            <a href="#">スタッフ</a>
          </li>
        </ul>
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

  .footB .list-title {
    margin-top: 30px;
    margin-bottom: 0;
    border-bottom: 1px solid currentColor;
    font-size: 14px;
  }

  .footB ul {
    margin-top: 10px;
    margin-bottom: 20px;
    padding: 0;
    list-style-type: none;
  }

  .footB li a {
    display: block;
    padding: 5px;
    font-size: 12px;
    color: var(--text-bright-color);
    text-decoration: none;
  }

  .footB li a:hover {
    background-image: linear-gradient(
      rgba(0, 0, 0, 0.3),
      rgba(0, 0, 0, 0.3)
    );
  }
</style>
