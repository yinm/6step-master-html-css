<template>
  <header :class="{ noHeroImage: isNoHeroImage }">
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
            @click="toggleMenu"
          />
        </button>
      </div>
      <nav class="headB">
        <transition name="slide-fade">
          <ul v-show="isOpen">
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
        </transition>
      </nav>
    </div>
  </header>
</template>

<script>
export default {
  props: {
    isNoHeroImage: {
      type: Boolean,
      default: false,
    }
  },

  data() {
    return {
      isOpen: false
    }
  },

  methods: {
    toggleMenu() {
      this.isOpen = !this.isOpen
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

.noHeroImage {
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

.slide-fade-enter-active {
  transition: all .3s ease;
}
.slide-fade-enter, .slide-fade-leave-to {
  transform: translateY(10px);
  opacity: 0;
}
</style>
