<template>
  <section>
    <div class="container">
      <h2>お問い合わせ</h2>
      <p>ROGGERについてのご質問などがございましたら、下記の窓口よりお問い合わせください。</p>
      <div class="cards">
        <div class="card">
          <i class="fas fa-phone" />
          <h3>電話</h3>
          <a href="tel:000-1234-5678">000-1234-5678</a>
        </div>
        <div class="card">
          <i class="fas fa-envelope" />
          <h3>Eメール</h3>
          <a href="mailto:contact@logger.nett">contact@logger.nett</a>
        </div>
      </div>
    </div>
  </section>
</template>

<style scoped>
  .container {
    padding: 30px 10px;
    max-width: var(--middle-width);
    margin-left: auto;
    margin-right: auto;
  }

  body {
    font-size: 16px;
  }

  @media (max-width: 599px) {
    :root {
      font-size: 14px;
    }
  }

  @media (min-width: 600px) and (max-width: 799px) {
    :root {
      font-size: 16px;
    }
  }

  @media (min-width: 800px) {
    :root {
      font-size: 18px;
    }

    .cards {
      display: flex;
    }

    .card {
      flex: 1;
    }

    .card:not(:last-child) {
      margin-right: 20px;
    }
  }

  h2 {
    padding-left: 0.5rem;
    border-left: solid 0.75rem var(--accent-color);
    font-size: 2rem;
  }

  p {
    font-size: 1rem;
    line-height: 2;
  }

  .card {
    margin-top: 20px;
    padding: 1.3rem;
    border: solid 1px var(--gray-color);
    text-align: center;
  }

  .card i {
    padding: 1.1rem;
    border-radius: 50%;
    background-color: var(--main-color);
    color: var(--text-bright-color);
    font-size: 2.2rem;
  }

  .card h3 {
    margin-top: 17px;
    margin-bottom: 17px;
    font-size: 1.2rem;
  }

  .card a {
    font-size: 1.4rem;
    color: inherit;
    text-decoration: none;
  }
</style>
