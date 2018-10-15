<template>
  <section class="conD">
    <div class="container">
      <div class="photo" />
      <div class="text">
        <h2>ライフログで毎日の日常生活をもっと楽しむ</h2>
        <p>ふと気が付くと蓄積しているライフログ。ログを見返すといろいろなことが見えてきて、なんてことのない日常も楽しくなってきます。</p>
        <div class="cover">
          <a href="#">
            たとえばこんな楽しみ方が…
            <i class="fas fa-chevron-right" />
          </a>
        </div>
      </div>
    </div>
  </section>
</template>

<style scoped>
  .conD {
    margin: 40px 0;
  }

  .conD h2 {
    margin-top: 0;
    margin-bottom: 10px;
    font-size: 20px;
  }

  .conD p {
    margin-top: 0;
    margin-bottom: 20px;
    font-size: 14px;
    line-height: 1.8;
    opacity: 0.8;
  }

  .conD .cover {
    margin-top: 20px;
    padding: 3px;
    border: solid 1px #888;
    border-radius: 6px;
    width: 256px;
  }

  .conD a {
    display: inline-block;
    padding: 10px 30px;
    background-color: var(--accent-color);
    border-radius: 6px;
    color: var(--text-bright-color);
    font-size: 14px;
    text-decoration: none;
  }

  .conD a:hover {
    background-image: linear-gradient(
      rgba(255, 255, 255, 0.2),
      rgba(255, 255, 255, 0.2)
    );
  }

  .conD .photo {
    min-height: 200px;
    background-image: url("/life.jpg");
    background-position: center;
    background-size: cover;
  }

  .conD .text {
    padding: 20px;
  }

  @media (min-width: 768px) {
    .conD .container {
      display: flex;
      max-width: var(--large-width);
      margin-left: auto;
      margin-right: auto;
    }

    .conD .photo {
      flex: 3;
    }

    .conD .text {
      flex: 2;
      padding: 50px;
    }
  }
</style>
