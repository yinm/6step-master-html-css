<template>
  <footer>
    <div class="container">
      <h2>LOGGER</h2>
      <p>
        〒000-0000 東京都中央区杉並3-3-3-403<br>
        <a href="#">http://logger.nett/</a>
      </p>

      <h3>ABOUT</h3>
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
  </footer>
</template>

<style scoped>
  footer {
    color: var(--text-bright-color);
    background-color: var(--dark-main-color);
  }

  .container {
    padding: 40px 20px;
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

  h3 {
    margin-top: 30px;
    margin-bottom: 10px;
    border-bottom: solid 1px currentColor;
    font-size: 14px;
  }

  ul {
    margin-top: 0;
    margin-bottom: 20px;
    padding-left: 0;
    list-style-type: none;
  }

  li a {
    display: block;
    padding: 5px;
    font-size: 12px;
  }

  li a:hover {
    background-image: linear-gradient(
      rgba(0, 0, 0, 0.3),
      rgba(0, 0, 0, 0.3)
    );
  }
</style>
