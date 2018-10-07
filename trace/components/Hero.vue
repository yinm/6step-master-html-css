<template>
  <section class="conA">
    <div class="container">
      <h1>LOGGER</h1>
      <p>美味しく楽しくライフログ</p>
    </div>
  </section>
</template>

<style scoped>
  @import url('https://fonts.googleapis.com/css?family=Montserrat');

  .conA {
    position: relative;
    background-image: url("/fruits.jpg");
    background-size: cover;
    background-position: center;
    width: 100vw;
    height: 100vh;
    text-align: center;
  }

  .conA::before {
    content: '';
    position: absolute;
    top: 0;
    right: 0;
    bottom: 0;
    left: 0;
    background-color: rgba(0, 0, 0, 0.2);
    z-index: -1;
  }

  .conA .container {
    position: relative;
    top: 40%;
  }

  .conA h1 {
    margin-top: 0;
    margin-bottom: 10px;
    font-size: 15vw;
    font-family: 'Montserrat', sans-serif;
    letter-spacing: 0.2em;
    margin-left: 0.2em;
    color: #fff;
  }

  .conA p {
    margin-top: 0;
    margin-bottom: 0;
    font-size: 18px;
    color: #fff;
  }

  @media (min-width: 768px) {
    .conA h1 {
      font-size: 115px;
    }

    .conA p {
      font-size: 24px;
    }
  }
</style>
