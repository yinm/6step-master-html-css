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
    </div>
  </footer>
</template>

<style scoped>
  @import url('https://fonts.googleapis.com/css?family=Montserrat');

  .footA {
    padding: 50px 20px;
    color: var(--text-bright-color);
    background-color: var(--dark-main-color);
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
</style>
