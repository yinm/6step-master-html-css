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
  .container {
    padding-top: 2px;
  }

  .text {
    padding: 20px;
  }

  h2 {
    margin-top: 0;
    margin-bottom: 10px;
    font-size: 20px;
  }

  p {
    margin-top: 0;
    margin-bottom: 20px;
    font-size: 14px;
    line-height: 1.8;
    opacity: 0.8;
  }

  a {
    display: inline-block;
    margin-top: 20px;
    padding: 10px 30px;
    box-shadow: 0 0 0 1px #888;
    border: solid 3px currentColor;
    border-radius: 6px;
    background-color: var(--accent-color);
    color: var(--text-bright-color);
    font-size: 14px;
    text-decoration: none;
  }

  a:hover {
    background-image: linear-gradient(
      rgba(255, 255, 255, 0.2),
      rgba(255, 255, 255, 0.2)
    );
  }

  .photo {
    min-height: 200px;
    background-image: url(/life.jpg);
    background-position: center;
    background-size: cover;
  }

  @media (min-width: 768px) {
    .container {
      display: flex;
      flex-direction: row-reverse;
      max-width: var(--large-width);
      margin-left: auto;
      margin-right: auto;
      padding-top: 40px;
      padding-bottom: 40px;
    }

    .photo {
      flex: 0 1 400px;
    }

    .text {
      flex: 2;
      padding: 50px;
    }
  }
</style>
