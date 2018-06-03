<template>
    <div id="accountlistcell">
        <div id="accountlistcellcontent">
            <div class="content-flex">
                <span class="leftcontent">{{ accounttype }}</span>
                <span class="rightcontent" style="font-weight: 600">{{ account }}</span>
            </div>
            <div class="content-flex">
                <span class="leftcontent">{{ time }}</span>
                <span class="rightcontent">{{ user }}</span>
            </div>
        </div>
        <div class="line"></div>
    </div>
</template>

<script type="text/babel">
  export default {
    name: 'AccountListCell',

    props: {
      accounttype: String,
      account: String,
      time: String,
      user: String,
    //   islastcell: Boolean
    }
  };
</script>

<style scoped>
#accountlistcellcontent {
    padding-left: 12px;
    padding-right: 12px;
    margin-top: 16px;
    margin-bottom: 16px;
}

.content-flex {
    display: flex;
    margin-top: 8px;
    margin-bottom: 8px;
}

.leftcontent {
    flex: 1;
    text-align: left;
}

.rightcontent {
    flex: 1;
    text-align: right;
}

.line{  
    text-align: center;
    background: #cccccc;
    height: 1px;
}
</style>
