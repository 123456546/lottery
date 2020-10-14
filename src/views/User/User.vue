<template>
  <div class="home">
    <Header msg="个人中心" iconRight="setting-o"/>
    <van-cell center  title label="1,000,000" icon class="top_user" is-link to="User/DetailUser">
      <template #right-icon>
        <van-icon name="arrow" class="arrow" />
      </template>
      <template #title>
        <span >test2020</span>
        <van-tag type="success" class="custom_info">VIP 0</van-tag>
      </template>
       <template #icon>
        <img alt="user_avatar" src='@/assets/user/icone_top.png'>
      </template>
    </van-cell>
    <van-grid direction="horizontal" :column-num="2" class="info_user">
      <van-grid-item icon text >
        <template #icon>
          <img alt="user_avatar" src='@/assets/user/icone9.png'>
        </template>
        <template #text>
          <h5 >VIP特权 <br><span>VIP PRIVILEGE</span></h5>
        </template>
      </van-grid-item>
      <van-grid-item icon text >
        <template #icon>
          <img alt="user_avatar" src='@/assets/user/icone8.png'>
        </template>
        <template #text>
          <h5 >积分兑换<br><span>exchange</span></h5>
        </template>
      </van-grid-item>
    </van-grid>
    <van-grid class="icone_info_user">
      <van-grid-item icon text="我的钱包" >
        <template #icon>
          <img alt="user_avatar" src='@/assets/user/icone_top1.png'>
        </template>
      </van-grid-item>
      <van-grid-item icon text="投注记录">
        <template #icon>
          <img alt="user_avatar" src='@/assets/user/icone_top3.png'>
        </template>
      </van-grid-item>
      <van-grid-item icon text="交易记录">
        <template #icon>
          <img alt="user_avatar" src='@/assets/user/icone_top2.png'>
        </template>
      </van-grid-item>
      <van-grid-item icon text="每日签到">
        <template #icon>
          <img alt="user_avatar" src='@/assets/user/icone_top4.png'>
        </template>
      </van-grid-item>
    </van-grid>
    <van-cell-group class="link_user">
      <van-cell center  title="代理中心" icon>
        <template #right-icon>
          <van-icon name="arrow" class="arrow" />
        </template>
        <template #icon>
          <img alt="user_avatar" src='@/assets/user/icone6.png'>
        </template>
      </van-cell>
      <van-cell center  title="安全中心" icon>
        <template #right-icon>
          <van-icon name="arrow" class="arrow" />
        </template>
        <template #icon>
          <img alt="user_avatar" src='@/assets/user/icone5.png'>
        </template>
      </van-cell>
      <van-cell center  title="在线客服" icon>
        <template #right-icon>
          <van-icon name="arrow" class="arrow" />
        </template>
        <template #icon>
          <img alt="user_avatar" src='@/assets/user/icone4.png'>
        </template>
      </van-cell>
      <van-cell center  title="分享App" icon>
        <template #right-icon>
          <van-icon name="arrow" class="arrow" />
        </template>
        <template #icon>
          <img alt="user_avatar" src='@/assets/user/icone3.png'>
        </template>
      </van-cell>
      <van-cell center  title icon>
        <template #right-icon>
          <van-icon name="arrow" class="arrow" />
        </template>
        <template #icon>
          <img alt="user_avatar" src='@/assets/user/icone2.png'>
        </template>
        <template #title>
        <span >主题换肤</span>
        <van-tag type="danger">New</van-tag>
      </template>
      </van-cell>
      <van-cell center  title="打开App" icon>
        <template #right-icon>
          <van-icon name="arrow" class="arrow" />
        </template>
        <template #icon>
          <img alt="user_avatar" src='@/assets/user/icone1.png'>
        </template>
      </van-cell>
    </van-cell-group>
    <Footer/>
  </div>
</template>

<script>
// @ is an alias to /src
import Header from '@/components/Header.vue'
import Footer from '@/components/Footer.vue'

export default {
  name: 'User',
  components: {
    Header,
    Footer
  }
}
</script>