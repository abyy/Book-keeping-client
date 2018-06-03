<template>
    <div id="accountlist">
        <div v-for="item in items" :key = "item.id">{{ item.msg }}</div>
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
    data() {
        return {items: [
            {msg: '123'},
            {msg: '321'}
        ]}
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
