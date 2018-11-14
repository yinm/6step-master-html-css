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
        >
          <i
            class="fas fa-bars"
            title="MENU"
          />
        </button>
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

ul {
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

li a:hover {
  background-color: rgba(0, 0, 0, 0.3);
}

@media (min-width: 768px) {
  .container {
    display: flex;
    align-items: center;
    justify-content: space-between;
    max-width: 1000px;
    margin-left: auto;
    margin-right: auto;
  }

  ul {
    display: flex;
  }

  .headC {
    display: none;
  }
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
</style>
