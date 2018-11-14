<template>
  <header>
    <div class="container">
      <div class="logo-wrapper">
        <a
          href="index.html"
          class="headA"
        >
          LOGGER
        </a>
        <i class="fas fa-bars" />
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

.logo-wrapper {
  display: flex;
  justify-content: space-between;
  align-items: center;
}

i {
  margin-right: 10px;
  font-size: 26px;
  color: #777;
}

i:hover {
  opacity: 0.6;
  cursor: pointer;
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

  i {
    display: none;
  }
}
</style>
