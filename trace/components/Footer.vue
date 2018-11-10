<template>
  <footer>
    <div class="container">
      <h2>LOGGER</h2>
      <p>
        〒000-0000 東京都中央区杉並3-3-3-403<br>
        <a href="#">http://logger.nett/</a>
      </p>
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
</style>
