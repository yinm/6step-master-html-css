<template>
  <section>
    <div class="container">
      <div class="photo" />
      <table class="history">
        <th class="history-title">History</th>
        <tr>
          <td class="history-date">2010年4月</td>
          <td class="history-text">LOGGER設立</td>
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
  </section>
</template>

<style scoped>
  section {
    background-color: var(--main-color);
  }

  .photo {
    min-height: 200px;
    background-image: url("/plant.jpg");
    background-position: center;
    background-size: cover;
  }

  .history {
    color: var(--text-bright-color);
  }

  .history-title {
    border-bottom: solid 1px currentColor;
  }

  .history tr {
    border-bottom: solid 1px currentColor;
  }

  @media (min-width: 800px) {
    .container {
      display: flex;
      max-width: var(--large-width);
      margin-left: auto;
      margin-right: auto;
    }

    .photo {
      flex: 3;
    }

    .history {
      flex: 2;
      padding: 50px;
    }
  }
</style>
