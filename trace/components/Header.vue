<template>
  <header>
    <div class="container">
      <div class="container-small">
        <a
          href="index.html"
          class="headA"
        >
          LOGGER
        </a>

        <button
          type="button"
          class="headC"
          @click="onClick"
        >
          <i class="fas fa-bars" />
          <span class="sr-only">MENU</span>
        </button>
      </div>

      <nav
        v-if="!isHidden"
        class="headB"
      >
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
    data() {
      return {
        isHidden: true,
      }
    },

    methods: {
      onClick() {
        this.isHidden = !this.isHidden
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
    .container-small {
      display: flex;
      align-items: center;
      justify-content: space-between;
    }

    .headC {
      margin-right: 10px;
      padding: 0;
      border: none;
      outline: none;
      background: none;
      font-size: 28px;
      opacity: 0.5;
      cursor: pointer;
    }

    .headC:hover {
      opacity: 0.3;
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

    .headC {
      display: none;
    }
  }
</style>
