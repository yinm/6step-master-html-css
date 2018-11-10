<template>
  <section class="conD">
    <div class="container">
      <div class="photo" />
      <div class="text">
        <h2>ライフログで毎日の日常生活をもっと楽しむ</h2>
        <p>ふと気が付くと蓄積しているライフログ。ログを見返すといろいろなことが見えてきて、なんてことのない日常も楽しくなってきます。</p>
        <a href="#">
          たとえばこんな楽しみ方が…
          <i class="fas fa-chevron-right" />
        </a>
      </div>
    </div>
  </section>
</template>

<style scoped>
  .conD {
    margin-top: 2px;
  }

  h2 {
    margin-top: 0;
    margin-bottom: 10px;
    font-size: 20px;
  }

  p {
    margin-top: 0;
    margin-bottom: 40px;
    font-size: 14px;
    line-height: 1.8;
    opacity: 0.8;
  }

  a {
    display: inline-block;
    padding: 10px 30px;
    border: solid 3px currentColor;
    border-radius: 6px;
    box-shadow: 0 0 1px #000;
    background-color: var(--accent-color);
    color: var(--text-bright-color);
    text-decoration: none;
    font-size: 14px;
  }

  .photo {
    min-height: 200px;
    background-image: url(/life.jpg);
    background-position: center;
    background-size: cover;
  }

  .text {
    padding: 20px;
  }

  @media (min-width: 768px) {
    .conD {
      margin-top: 40px;
      margin-bottom: 40px;
    }

    .container {
      display: flex;
      max-width: var(--large-width);
      margin-left: auto;
      margin-right: auto;
    }

    .photo {
      flex: 3;
    }

    .text {
      flex: 2;
      padding: 50px;
    }
  }
</style>
