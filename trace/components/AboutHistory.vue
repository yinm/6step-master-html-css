<template>
  <section>
    <div class="container">
      <div class="photo" />
      <div class="history-container">
        <h2>History</h2>
        <table>
          <tr>
            <td>2010年4月</td>
            <td>LOGGER設立</td>
          </tr>
          <tr>
            <td>2012年6月</td>
            <td>オンラインマガジン創刊</td>
          </tr>
          <tr>
            <td>2014年12月</td>
            <td>海外企業と提携してオンラインデータ共有事業をスタート</td>
          </tr>
          <tr>
            <td>2015年1月</td>
            <td>ライフログアプリをリリース</td>
          </tr>
        </table>
      </div>
    </div>
  </section>
</template>

<style scoped>
section {
  background-color: var(--main-color);
  color: var(--text-bright-color);
}

.photo {
  min-height: 300px;
  background-image: url(/plant.jpg);
  background-position: center;
  background-size: cover;
}

.history-container {
  padding: 10px 20px;
}

h2 {
  margin-bottom: 7px;
}

tr {
  display: block;
  padding-top: 30px;
  padding-bottom: 25px;
  border-top: solid 1px currentColor;
  font-size: 0.875rem;
}

tr:last-child {
  padding-bottom: 30px;
  border-bottom: solid 1px currentColor;
}

td:first-child {
  font-weight: bold;
  min-width: 110px;
}

@media (min-width: 768px) {
  .container {
    display: flex;
    padding: 0 30px;
    justify-content: space-between;
  }

  .photo {
    flex: 3;
  }

  .history-container {
    flex: 2;
    padding: 30px 50px;
  }
}
</style>
