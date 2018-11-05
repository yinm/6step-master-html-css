<template>
  <section class="conA">
    <div class="container">
      <svg
        xmlns="http://www.w3.org/2000/svg"
        viewBox="0 0 100 100"><defs><style>.a{fill:none;stroke:#fff;stroke-width:6.59px;}</style></defs><title>logo-color</title><rect
          class="a"
          x="18.44"
          y="18.28"
          width="64.05"
          height="64.05"
          transform="translate(-21.09 49.72) rotate(-45)"/><line
            class="a"
            x1="48.86"
            y1="6.58"
            x2="48.86"
            y2="70.62"/><line
              class="a"
              x1="28.5"
              y1="26.64"
              x2="28.5"
              y2="70.06"/><line
                class="a"
                x1="29.87"
                y1="49.6"
                x2="92.14"
                y2="49.6"/><line
                  class="a"
                  x1="25.2"
                  y1="70.62"
                  x2="73.92"
                  y2="70.62"/></svg>
      <h1>LOGGER</h1>
      <p>美味しく楽しくライフログ</p>
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

  svg {
    width: 17vw;
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

  @media (min-width: 768px) {
    svg {
      width: 132px;
    }

    h1 {
      font-size: 115px;
    }

    p {
      font-size: 24px;
    }
  }
</style>
