<template>
    <div id="accountlist">
        <div v-for="value in object" :key = "value.id">{{ value }}</div>
        <!-- <AccountListCell accounttype="accounttype"
                         account="account"
                         time="time"
                         user="user"
            ></AccountListCell> -->
    </div>
</template>

<script type="text/babel">
  import AccountListCell from './AccountListCell.vue'
  export default {
    name: 'AccountList',
    data: {
        object: {
            a: 'a',
            b: 'b',
            c: 'c'
        }
    },

    props: {
      accountList: [
          
      ]
    },

    components: {
        AccountListCell
    }
  };
</script>

<style scoped>

</style>
