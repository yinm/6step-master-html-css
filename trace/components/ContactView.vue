<template>
  <div>
    <div class="container">
      <h1>お問い合わせ</h1>
      <p>ROGGERについてのご質問などがございましたら、下記の窓口よりお問い合わせください。</p>
      <div class="contact-wrap">
        <div class="card">
          <i class="fas fa-phone" />
          <h2>電話</h2>
          <p>000-1234-5678</p>
        </div>
        <div class="card">
          <i class="fas fa-envelope" />
          <h2>Eメール</h2>
          <p>contact@logger.nett</p>
        </div>
      </div>
    </div>
  </div>
</template>

<style scoped>
.container {
  max-width: var(--middle-width);
  margin-left: auto;
  margin-right: auto;
  padding: 50px 10px;
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

body {
  font-size: 16px;
}

h1 {
  margin-top: 10px;
  margin-bottom: 2rem;
  border-left: solid 0.75rem var(--accent-color);
  padding-left: 0.5rem;
  font-size: 2rem;
}

p {
  margin-top: 0;
  font-size: 1rem;
}

.contact-wrap {
  margin-top: 30px;
}

.card {
  margin-top: 20px;
  padding: 20px;
  border: solid 1px var(--gray-color);
  text-align: center;
}

i {
  border-radius: 50%;
  background-color: var(--main-color);
  color: var(--icon-color);
  font-size: 2.2rem;
  width: 2em;
  line-height: 2em;
  text-align: center;
}

h2 {
  font-size: 1.2rem;
}

.card p {
  margin: 0;
  font-size: 1.4rem;
}

@media (min-width: 800px) {
  .contact-wrap {
    display: flex;
  }

  .card {
    flex: 1;
  }

  .card:not(:last-child) {
    margin-right: 20px;
  }
}
</style>
