<template>
  <div class="home">
    <Header msg="娱乐大厅" :HomePage="HomePage"/>
    <van-swipe class="my-swipe" :autoplay="5000" indicator-color="white">
      <van-swipe-item><img alt="user_avatar" src='@/assets/home/banner1.png'></van-swipe-item>
      <van-swipe-item><img alt="user_avatar" src='@/assets/home/banner2.png'></van-swipe-item>
      <van-swipe-item><img alt="user_avatar" src='@/assets/home/banner4.png'></van-swipe-item>
    </van-swipe>
    <van-notice-bar text="公告：春节将近，为回馈广大新老玩家的支持，本平台现推出全..." left-icon class="notification_top">
      <template #left-icon>
        <img alt="" src='@/assets/home/notif.png'>
      </template>
    </van-notice-bar>
    <van-grid class="icone_info_user">
      <van-grid-item icon text="我的钱包" >
        <template #icon>
          <img alt="user_avatar" src='@/assets/home/topIcone1.png'>
        </template>
      </van-grid-item>
      <van-grid-item icon text="投注记录">
        <template #icon>
          <img alt="user_avatar" src='@/assets/home/topIcone2.png'>
        </template>
      </van-grid-item>
      <van-grid-item icon text="交易记录">
        <template #icon>
          <img alt="user_avatar" src='@/assets/home/topIcone3.png'>
        </template>
      </van-grid-item>
      <van-grid-item icon text="每日签到">
        <template #icon>
          <img alt="user_avatar" src='@/assets/home/topIcone4.png'>
        </template>
      </van-grid-item>
    </van-grid>
    <Footer/>
  </div>
</template>

<script>
import Header from '@/components/Header.vue'
import Footer from '@/components/Footer.vue'
export default {
  name: 'Home',
  components: {
      Header,
      Footer
  },
  data() {
    return {
      HomePage:true,
    }
  }
}
</script>
