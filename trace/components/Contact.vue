<template>
  <article class="post">
    <div class="container">
      <h1>お問い合わせ</h1>
      <p>ROGGERについてのご質問などがございましたら、下記の窓口よりお問い合わせください。</p>

      <div class="contact-wrap">
        <div class="contact">
          <i class="fas fa-phone" />
          <h2>電話</h2>
          <a href="tel:000-1234-5678">000-1234-5678</a>
        </div>

        <div class="contact">
          <i class="fas fa-envelope" />
          <h2>Eメール</h2>
          <a href="mailto:contact@logger.nett">contact@logger.nett</a>
        </div>
      </div>
    </div>
  </article>
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
  }

  h1 {
    padding-left: 0.5rem;
    border-left: solid 0.75rem var(--accent-color);
    font-size: 2rem;
  }

  p {
    font-size: 1rem;
    line-height: 2;
  }

  .contact {
    margin-top: 20px;
    margin-bottom: 20px;
    padding: 20px;
    border: solid 1px var(--gray-color);
    text-align: center;
  }

  .contact i {
    display: inline-block;
    margin-bottom: 20px;
    font-size: 2.2rem;
    width: 2em;
    line-height: 2em;
    border-radius: 50%;
    text-align: center;
    background-color: var(--main-color);
    color: var(--icon-color);
  }

  .contact h2 {
    margin-top: 0;
    font-size: 1.2rem;
  }

  .contact a {
    font-size: 1.4rem;
    color: inherit;
    text-decoration: none;
  }

  @media (min-width: 768px) {
    .contact-wrap {
      display: flex;
    }

    .contact {
      flex: 1;
    }

    .contact:first-child {
      margin-right: 20px;
    }
  }
</style>
