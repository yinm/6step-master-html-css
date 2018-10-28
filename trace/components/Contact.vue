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

    <section class="map">
      <h2>LOCATION</h2>
      <iframe
        src="https://www.google.com/maps/embed?pb=!1m18!1m12!1m3!1d3239.6566075690303!2d139.80851171557487!3d35.71006703599668!2m3!1f0!2f0!3f0!3m2!1i1024!2i768!4f13.1!3m3!1m2!1s0x60188ed6f9ddd30f%3A0x918ba47a310c8809!2z5p2x5Lqs44K944Op44Oe44OB!5e0!3m2!1sja!2sjp!4v1540707001406"
        frameborder="0"
        style="border:0"
        allowfullscreen/>
    </section>
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

  .map h2 {
    margin: 0;
    padding: 20px;
    background-color: var(--main-color);
    color: var(--text-bright-color);
    text-align: center;
  }

  iframe {
    width: 100%;
    height: 395px;
  }
</style>
