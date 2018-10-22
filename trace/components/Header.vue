<template>
  <header>
    <div class="container">
      <a
        href="index.html"
        class="headA"
      >
        LOGGER
      </a>

      <ul class="header-list">
        <li>
          <a href="#">トップ</a>
        </li>
        <li>
          <a href="#">コンテンツ</a>
        </li>
        <li>
          <a href="#">ABOUT</a>
        </li>
        <li>
          <a href="#">お問い合わせ</a>
        </li>
      </ul>
    </div>
  </header>
</template>

<style scoped>
  header {
    position: absolute;
    top: 0;
    left: 0;
    z-index: 100;
    width: 100%;
    background-color: rgba(255, 255, 255, 0.9);
  }

  .headA {
    display: inline-block;
    line-height: 70px;
    padding-left: 20px;
    padding-right: 20px;
    background-color: var(--main-color);
    color: var(--text-bright-color);
    font-family: 'Montserrat', sans-serif;
    font-size: 24px;
    text-decoration: none;
  }

  .header-list {
    margin: 0;
    padding: 0;
    list-style-type: none;
  }

  .header-list a {
    display: block;
    padding: 15px;
    text-decoration: none;
    color: inherit;
    font-size: 12px;
  }

  .header-list a:hover {
    background-color: rgba(0, 0, 0, 0.3);
  }
</style>
