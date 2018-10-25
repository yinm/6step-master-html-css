<template>
  <header :class="{nohero: !isHeroImage}">
    <div class="container">
      <div class="container-small">
        <a
          href="index.html"
          class="headA"
        >
          LOGGER
        </a>
      </div>

      <nav class="headB">
        <ul>
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
      </nav>
    </div>
  </header>
</template>

<script>
  export default {
    props: {
      isHeroImage: {
        type: Boolean,
        default: true,
      }
    }
  }
</script>

<style scoped>
  header {
    position: absolute;
    top: 0;
    left: 0;
    z-index: 100;
    width: 100%;
    background-color: rgba(255, 255, 255, 0.9);
  }

  .nohero {
    position: static;
    border-bottom: solid 1px var(--gray-color);
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

  .headB ul {
    margin: 0;
    padding: 0;
    list-style: none;
  }

  .headB a {
    display: block;
    padding: 15px;
    color: inherit;
    font-size: 12px;
    text-decoration: none;
  }

  .headB a:hover {
    background-color: rgba(0, 0, 0, 0.3);
  }

  @media (max-width: 767px) {
    .headB {
      display: none;
    }
  }

  @media (min-width: 768px) {
    .container {
      display: flex;
      align-items: center;
      justify-content: space-between;
      max-width: var(--large-width);
      margin-left: auto;
      margin-right: auto;
    }

    .headB ul {
      display: flex;
    }
  }
</style>
