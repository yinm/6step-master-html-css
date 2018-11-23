<template>
  <aside class="history">
    <div class="photo" />

    <div class="text">
      <h2>History</h2>
      <table>
        <tr>
          <th>2010年4月</th>
          <td>LOGGER設立</td>
        </tr>
        <tr>
          <th>2012年6月</th>
          <td>オンラインマガジン創刊</td>
        </tr>
        <tr>
          <th>2014年12月</th>
          <td>海外企業と提携してオンラインデータ共有事業をスタート</td>
        </tr>
        <tr>
          <th>2015年1月</th>
          <td>ライフログアプリをリリース</td>
        </tr>
      </table>
    </div>
  </aside>
</template>

<style scoped>
.history {
  background-color: var(--main-color);
  color: var(--text-bright-color);
}

.photo {
  min-height: 300px;
  background-image: url(/plant.jpg);
  background-position: center;
  background-size: cover;
}

.text {
  padding: 20px;
}

table {
  border-top: solid 1px var(--gray-color);
  border-collapse: collapse;
}

h2 {
  margin-top: 0;
  margin-bottom: 10px;
}

tr {
  height: 90px;
  font-size: 0.87rem;
}

th,
td {
  border-bottom: solid 1px var(--gray-color);
}

th {
  word-break: keep-all;
  text-align: left;
}

td {
  padding-left: 1rem;
}

@media (min-width: 768px) {
  .history {
    display: flex;
    padding-left: 35px;
    padding-right: 35px;
  }

  .photo {
    flex: 3;
  }

  .text {
    flex: 2;
    padding: 50px;
  }
}
</style>
