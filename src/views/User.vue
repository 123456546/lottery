<template>
  <div class="home">
    <Header msg="个人中心"/>
    <van-cell center  title label="1,000,000" icon class="top_user">
      <template #right-icon>
        <van-icon name="arrow" class="arrow" />
      </template>
      <template #title>
        <span >test2020</span>
        <van-tag type="success" class="custom_info">VIP 0</van-tag>
      </template>
       <template #icon>
        <img alt="user_avatar" src="../assets/user/icone_top.png">
      </template>
    </van-cell>
    <van-grid direction="horizontal" :column-num="2" class="info_user">
      <van-grid-item icon text >
        <template #icon>
          <img alt="user_avatar" src="../assets/user/icone9.png">
        </template>
        <template #text>
          <h5 >VIP特权 <br><span>VIP PRIVILEGE</span></h5>
        </template>
      </van-grid-item>
      <van-grid-item icon text >
        <template #icon>
          <img alt="user_avatar" src="../assets/user/icone8.png">
        </template>
        <template #text>
          <h5 >积分兑换<br><span>exchange</span></h5>
        </template>
      </van-grid-item>
    </van-grid>
    <van-grid class="icone_info_user">
      <van-grid-item icon text="我的钱包" >
        <template #icon>
          <img alt="user_avatar" src="../assets/user/icone_top1.png">
        </template>
      </van-grid-item>
      <van-grid-item icon text="投注记录">
        <template #icon>
          <img alt="user_avatar" src="../assets/user/icone_top3.png">
        </template>
      </van-grid-item>
      <van-grid-item icon text="交易记录">
        <template #icon>
          <img alt="user_avatar" src="../assets/user/icone_top2.png">
        </template>
      </van-grid-item>
      <van-grid-item icon text="每日签到">
        <template #icon>
          <img alt="user_avatar" src="../assets/user/icone_top4.png">
        </template>
      </van-grid-item>
    </van-grid>
    <van-cell-group class="link_user">
      <van-cell center  title="代理中心" icon>
        <template #right-icon>
          <van-icon name="arrow" class="arrow" />
        </template>
        <template #icon>
          <img alt="user_avatar" src="../assets/user/icone6.png">
        </template>
      </van-cell>
      <van-cell center  title="安全中心" icon>
        <template #right-icon>
          <van-icon name="arrow" class="arrow" />
        </template>
        <template #icon>
          <img alt="user_avatar" src="../assets/user/icone5.png">
        </template>
      </van-cell>
      <van-cell center  title="在线客服" icon>
        <template #right-icon>
          <van-icon name="arrow" class="arrow" />
        </template>
        <template #icon>
          <img alt="user_avatar" src="../assets/user/icone4.png">
        </template>
      </van-cell>
      <van-cell center  title="分享App" icon>
        <template #right-icon>
          <van-icon name="arrow" class="arrow" />
        </template>
        <template #icon>
          <img alt="user_avatar" src="../assets/user/icone3.png">
        </template>
      </van-cell>
      <van-cell center  title icon>
        <template #right-icon>
          <van-icon name="arrow" class="arrow" />
        </template>
        <template #icon>
          <img alt="user_avatar" src="../assets/user/icone2.png">
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
          <img alt="user_avatar" src="../assets/user/icone1.png">
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
  name: 'Home',
  components: {
    Header,
    Footer
  }
}
</script>
<style >
.custom-title {
    margin-right: 4px;
    vertical-align: middle;
  }

  .search-icon {
    font-size: 16px;
    line-height: inherit;
  }
  .top_user>img {
    width: 50px;
    border-radius: 50%;
    display: inline-block;
}

.top_user .van-cell__title {
    flex: initial;
    text-align: left;
    padding-left: 15px;
    color: #363636;
}

.top_user .van-cell__title>div {
    margin: 0;
    color: #959595;
}

.top_user .van-icon {
    float: right;
    flex: 1;
    text-align: right;
    color: #bfc3cf;
}
.top_user {
    padding: 10px 5px;
}
.top_user::after{
  display: none;
}
span.custom_info {
    margin-left: 5px;
    background: #e7caaa;
    color: #794a16;
    font-size: 13px;
    font-weight: bold;
    text-transform: uppercase;
    padding: 2px 5px;
}
.home {
    background: #fefefe;
}
.info_user img {
    width: 40px;
    margin-right: 6px;
}

.info_user h5 {
    /* width: 100%; */
    display: block;
    margin: 0;
    text-align: left;
}

.info_user p {
    display: block;
    width: 100%;
}

.info_user {
    text-align: center;
    box-shadow: 9px 6px 26px 6px #e9e9e9;
    margin-left: 5px;
    margin-right: 5px;
    border-radius: 6px;
    margin-bottom: 7px;
}
.info_user .van-grid-item__content{
  background: transparent;

}
.info_user h5 span {
    font-size: 9pt;
    font-weight: initial;
}

.info_user .van-grid-item {
    text-align: center;
}

.info_user .van-grid-item__content::after {
    border: none;
}

.info_user .van-grid-item:first-child .van-grid-item__content::before {
    content: '';
    border: 1px solid #c2c6d1;
    height: 58%;
    width: 0px;
    position: absolute;
    right: 0;
}
.icone_info_user img {
    width: 29px;
}

.icone_info_user .van-grid-item__content {
    padding: 10px;
}


.icone_info_user {
    background: #fff;
    border-bottom-left-radius: 12px;
    border-bottom-right-radius: 12px;
}
.icone_info_user .van-grid-item__content::after {
    border: none;
}
.link_user {
    background: #f2f4f8;
    padding-top: 10px;
    padding-bottom: 54px;
}

.link_user img {
    width: 16px;
}

.link_user .van-cell__title {
    text-align: left;
    padding-left: 15px;
}

.link_user .van-cell::after {
    right: 0;
    left: 0;
}
.link_user span.van-tag {
    margin-left: 10px;
}
.link_user .van-icon {
    color: #bdc1ce;
}
</style>