<template>
  <aside class="history">
    <div class="container">
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
    </div>
  </aside>
</template>

<style scoped>
.history {
  background-color: var(--main-color);
  color: var(--text-bright-color);
}

.text {
  padding: 20px;
}

h2 {
  margin-top: 0;
  margin-bottom: 10px;
  font-size: 1.5rem;
}

.photo {
  min-height: 300px;
  background-image: url(/plant.jpg);
  background-position: center;
  background-size: cover;
}

table {
  border-collapse: collapse;
  border-top: solid 1px var(--gray-color);
  font-size: 0.875rem;
}

th,
td {
  padding-top: 1.8rem;
  padding-bottom: 1.8rem;
  border-bottom: solid 1px var(--gray-color);
}

th {
  padding-right: 1rem;
  text-align: left;
  word-break: keep-all;
}

@media (min-width: 768px) {
  .container {
    display: flex;
    max-width: var(--large-width);
    margin-left: auto;
    margin-right: auto;
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
