<template>
  <!-- ref: http://lab.astamuse.co.jp/entry/2018/10/15/154737 -->
  <div class="container">
    <div class="accordion-container">
      <button
        type="button"
        class="accordion-opener is-opened"
      >
        アコーディオン1
      </button>
      <div class="accordion-body">
        <p>アコーディオンの中身</p>
        <p>アコーディオンの中身</p>
        <p>アコーディオンの中身</p>
      </div>
    </div>

    <div class="accordion-container">
      <button
        type="button"
        class="accordion-opener"
      >
        アコーディオン1
      </button>
      <div class="accordion-body">
        <p>アコーディオンの中身</p>
        <p>アコーディオンの中身</p>
        <p>アコーディオンの中身</p>
      </div>
    </div>
  </div>
</template>

<style scoped>
.container {
  padding: 20px;
  width: 80vw;
  margin: 0 auto;
}

.accordion-container {
  border-color: #666;
  border-style: solid;
  border-width: 1px 1px 0 1px;
  border-radius: 2px;
}

.accordion-container:last-child {
  border-bottom-width: 1px;
}

.accordion-opener {
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

.accordion-opener::after {
  position: absolute;
  top: 50%;
  right: 1em;
  display: inline-block;
  margin-top: -5px;
  width: 0;
  height: 0;
  border: solid 7px transparent;
  content: '';
  border-top-color: #5f6569;
  transition: all 0.2s ease-in;
}

.accordion-opener:hover,
.accordion-opener.is-opened {
  background-color: #999;
  text-decoration: none;
}

.accordion-opener.is-opened::after {
  transform: rotateX(180deg);
  margin-top: -10px;
}

.accordion-body {
  padding: 30px;
  overflow: hidden;
  transition: 0.4s ease-in-out;
}
</style>


