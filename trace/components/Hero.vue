<template>
  <section class="conA">
    <div class="container">
      <img
        src="/logo.svg"
        alt=""
      >
      <h1>LOGGER</h1>
      <p>美味しく楽しくライフログ</p>
      <a href="#">ライフログを始める</a>
    </div>
  </section>
</template>

<style scoped>
  @import url('https://fonts.googleapis.com/css?family=Montserrat');

  .conA {
    display: flex;
    justify-content: center;
    align-items: center;
    height: 100vh;
    min-height: 450px;
    background-image: linear-gradient(
      rgba(0, 0, 0, 0.1),
      rgba(0, 0, 0, 0.1)
    ), url("/fruits.jpg");
    background-position: center;
    background-size: cover;
    text-align: center;
    color: var(--text-bright-color);
  }

  img {
    width: 20%;
  }

  h1 {
    margin-top: 0;
    margin-bottom: 10px;
    font-family: 'Montserrat', sans-serif;
    font-size: 15vw;
    letter-spacing: 0.2em;
    margin-left: 0.2em;
  }

  p {
    margin-top: 0;
    margin-bottom: 0;
    font-size: 18px;
  }

  a {
    display: inline-block;
    margin-top: 20px;
    padding: 10px 30px;
    border: solid 3px currentColor;
    border-radius: 6px;
    background-color: var(--accent-color);
    font-size: 14px;
    color: var(--text-bright-color);
    text-decoration: none;
  }

  a:hover {
    background-image: linear-gradient(rgba(255, 255, 255, 0.2), rgba(255, 255, 255, 0.2));
  }

  @media (min-width: 768px) {
    h1 {
      font-size: 115px;
    }

    p {
      font-size: 24px;
    }
  }
</style>
