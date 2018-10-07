<template>
  <div class="hero-container">
    <h1 class="hero-title">LOGGER</h1>
    <p class="hero-subtitle">美味しく楽しくライフログ</p>
  </div>
</template>

<style scoped>
  .hero-title {
    margin: 0;
    text-align: center;
    font-size: 7.2rem;
    font-family: "Hiragino Kaku Gothic Pro";
  }

  .hero-subtitle {
    margin-top: 10px;
    margin-bottom: 0;
    text-align: center;
    font-size: 1.5rem;
    font-family: "Hiragino Kaku Gothic Pro";
  }

  @media (max-width: 768px) {
    .hero-title {
      font-size: 15vw;
    }
    .hero-subtitle {
      font-size: 3.5vw;
    }
  }
</style>
