<template>
    <div id="accountinfo">
        <div class="content-account" style="font-size: 1.3em">
            <p class="text-account">￥{{ curMonthPaid }}</p>
            <p class="text-curmonth">{{ curMonth }}月支出</p>
        </div>
        <div class="content-account">
            <p class="text-account">￥{{ curMonthAccount }}</p>
            <p class="text-curmonth">{{ curMonth }}月结余</p>
        </div>
    </div>
</template>

<script type="text/babel">
  export default {
    name: 'AccountInfo',

    props: {
      curMonthAccount: String,
      curMonthPaid: String,
      curMonth: String
    }
  };
</script>

<style scoped>
#accountinfo {
    background-color: #409EFF;
    color: #fff;
    padding-top: 12px;
    padding-bottom: 12px;
}

.content-half {
    /* display: flex; */
    width: 50%;
}

p {
    margin-top: 4px;
    margin-bottom: 4px;
}

.content-account {
    margin-top: 28px;
    margin-bottom: 28px;
}

.text-curmonth {
    font-size: 0.75em;
}

.text-account {
    font-weight: 600;
}
</style>
