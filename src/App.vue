<template>
  <div id="app">
    <AccountInfo curMonth="6"
                curMonthAccount="20,372.85"
                curMonthPaid="3,482.75"
        ></AccountInfo>
    <AccountList type="0"></AccountList>
  </div>
</template>

<script>
import AccountInfo from './components/AccountInfo.vue'
import AccountList from './components/AccountList.vue'

export default {
  name: 'app',
  components: {
    AccountInfo,
    AccountList
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
  /* margin-top: 60px; */
}
</style>
