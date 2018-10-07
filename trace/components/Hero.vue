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
    text-align: center;
  }

  .conA h1 {
    margin-top: 0;
    margin-bottom: 10px;
    font-size: 15vw;
    font-family: 'Montserrat', sans-serif;
    letter-spacing: 0.2em;
    margin-left: 0.2em;
  }

  .conA p {
    margin-top: 0;
    margin-bottom: 0;
    font-size: 18px;
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
