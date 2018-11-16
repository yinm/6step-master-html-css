<template>
  <!-- ref: http://lab.astamuse.co.jp/entry/2018/10/15/154737 -->
  <div class="js-accordion">
    <button
      :class="{ '_state-open': isOpened }"
      type="button"
      class="js-accordion--trigger"
      @click="accordionToggle"
    >
      アコーディオン1
    </button>
    <div
      v-if="isOpened"
      :class="{ '_state-open': isOpened }"
      class="js-accordion--target"
    >
      <div class="js-accordion--body">
        <p>アコーディオン1の中身</p>
        <p>アコーディオン1の中身</p>
        <p>アコーディオン1の中身</p>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  data() {
    return {
      isOpened: false
    }
  },

  methods: {
    accordionToggle() {
      this.isOpened = !this.isOpened
    }
  }
}
</script>

<style>
body {
  margin: 0;
  font-family: 'メイリオ', 'Hiragino Kaku Gothic Pro', sans-serif;
}

.js-accordion {
  background-color: #fff;
  border-color: #666;
  border-style: solid;
  border-width: 1px 1px 0 1px;
  border-radius: 2px;
}

.js-accordion:last-child {
  border-bottom-width: 1px;
}

.js-accordion--trigger {
  position: relative;
  display: block;
  background-color: #f1f1f1;
  width: 100%;
  transition: all 0.2s ease-in;
  color: #4d68b7;
  font-size: 20px;
  font-weight: bold;
  text-align: left;
  padding: 20px;
  outline: none;
  border: none;
  cursor: pointer;
}

.js-accordion--trigger::after {
  position: absolute;
  top: 50%;
  right: 1em;
  margin-top: -5px;
  display: inline-block;
  width: 0;
  height: 0;
  border: solid transparent;
  content: '';
  border-top-color: #5f6569;
  border-width: 7px;
  transition: all 0.2s ease-in;
}

.js-accordion--trigger._state-open {
  background-color: #999;
  text-decoration: none;
}

.js-accordion--trigger._state-open::after {
  transform: rotateX(180deg);
  margin-top: -10px;
}

.js-accordion--trigger:hover {
  background-color: #999;
  text-decoration: none;
}

.js-accordion--target {
  overflow: hidden;
  transition: 0.4s ease-in-out;
}

.js-accordion--body {
  padding: 10px;
}
</style>
