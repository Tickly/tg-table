<template>
  <div id="app">
    <tg-table :data="GroupData" bordered>
      <tg-table-column attr="kkhgl" />
      <tg-table-column attr="qy" />
      <tg-table-column attr="nylx" />
      <tg-table-column attr="scjc" />
      <tg-table-column attr="dqz" />
      <tg-table-column attr="tqz" />
    </tg-table>
  </div>
</template>

<script>
import TgTable from './Table'
import TgTableColumn from './TableColumn'
import GroupData from './data/group'

export default {
  name: 'App',
  components: { TgTable, TgTableColumn },
  data() {
    return {
      GroupData
    }
  }
}
</script>

<style>
#app {
  font-family: 'Avenir', Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
