<template>
    <van-tabbar v-model="active" active-color="#3889ff" inactive-color="#999999">
        <van-tabbar-item icon="wap-home">游戏大厅</van-tabbar-item>
        <van-tabbar-item icon="gift-card">优惠活动</van-tabbar-item>
        <van-tabbar-item icon="add" class="center_tab"></van-tabbar-item>
        <van-tabbar-item icon="label">开奖结果</van-tabbar-item>
        <van-tabbar-item icon="manager">个人中心</van-tabbar-item>
    </van-tabbar>
</template>
<script>

export default {
  name: 'Footer',
  data() {
    return {
      active: 0,
      icon: {
        active: 'https://img.yzcdn.cn/vant/user-active.png',
        inactive: 'https://img.yzcdn.cn/vant/user-inactive.png',
      },
    }
  }
}
</script>
<style >
.center_tab .van-icon {
    color: #3570f7;
    font-size: 44pt;
    position: relative;
    top: -8px;
    background: #fff;
    border-radius: 50%;
    border-top: 1px solid #ebedf0;
    /* box-shadow: -1px -12px 24px 0px #ccc; */
    z-index: 1;
}
</style>