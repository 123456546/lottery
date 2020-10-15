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
    <van-tree-select height="75vw" :items="items" :main-active-index.sync="active">
      <template #content>
        <div class="content_home_grup" v-if="active === 0">
            <div class="content_header">
              <h2>天津时时彩</h2>
              <p>momoLOTTERY</p>
                    <img alt="user_avatar" src='@/assets/home/sucai.png'>
                    <van-button plain>开始游戏</van-button>
            </div>
            <van-grid :gutter="10" direction="horizontal" :column-num="2" >
              <van-grid-item text class="block1">
                <template #text>
                  <p>
                    天津时时彩
                  </p>
                  <div>
                    <h2>天津时时彩</h2>
                    <van-button plain>XX分钟一期</van-button>
                    <img alt="user_avatar" src='@/assets/home/超级3D.png'>
                  </div>
                </template>
              </van-grid-item>
              <van-grid-item text class="block2">
                <template #text>
                  <p>
                    天津时时彩
                  </p>
                  <div>
                    <h2>天津时时彩</h2>
                    <van-button plain>XX分钟一期</van-button>
                    <img alt="user_avatar" src='@/assets/home/十分六合彩.png'>
                  </div>
                </template>
              </van-grid-item>
              <van-grid-item text class="block3">
                <template #text>
                  <p>
                    天津时时彩
                  </p>
                  <div>
                    <h2>天津时时彩</h2>
                    <van-button plain>XX分钟一期</van-button>
                    <img alt="user_avatar" src='@/assets/home/十分快三.png'>
                  </div>
                </template>
              </van-grid-item>
              <van-grid-item text class="block4">
                <template #text>
                  <p>
                    天津时时彩
                  </p>
                  <div>
                    <h2>天津时时彩</h2>
                    <van-button plain>XX分钟一期</van-button>
                    <img alt="user_avatar" src='@/assets/home/湖北快三.png'>
                  </div>
                </template>
              </van-grid-item>
              <van-grid-item text class="block5">
                <template #text>
                  <p>
                    天津时时彩
                  </p>
                  <div>
                    <h2>天津时时彩</h2>
                    <van-button plain>XX分钟一期</van-button>
                    <img alt="user_avatar" src='@/assets/home/天津时时彩.png'>
                  </div>
                </template>
              </van-grid-item>
              <van-grid-item text class="block6">
                <template #text>
                  <p>
                    天津时时彩
                  </p>
                  <div>
                    <h2>天津时时彩</h2>
                    <van-button plain>XX分钟一期</van-button>
                    <img alt="user_avatar" src='@/assets/home/一分11选5.png'>
                  </div>
                </template>
              </van-grid-item>
            </van-grid>
        </div>
        
        <div class="content_home_grup" v-if="active === 1">
            <div class="content_header">
              <h2>天津时时彩</h2>
              <p>momoLOTTERY</p>
                    <img alt="user_avatar" src='@/assets/home/sucai.png'>
                    <van-button plain>开始游戏</van-button>
            </div>
            <van-grid :gutter="10" direction="horizontal" :column-num="2" >
              <van-grid-item text class="block1">
                <template #text>
                  <p>
                    天津时时彩
                  </p>
                  <div>
                    <h2>天津时时彩</h2>
                    <van-button plain>XX分钟一期</van-button>
                    <img alt="user_avatar" src='@/assets/home/超级3D.png'>
                  </div>
                </template>
              </van-grid-item>
              <van-grid-item text class="block2">
                <template #text>
                  <p>
                    天津时时彩
                  </p>
                  <div>
                    <h2>天津时时彩</h2>
                    <van-button plain>XX分钟一期</van-button>
                    <img alt="user_avatar" src='@/assets/home/十分六合彩.png'>
                  </div>
                </template>
              </van-grid-item>
              <van-grid-item text class="block3">
                <template #text>
                  <p>
                    天津时时彩
                  </p>
                  <div>
                    <h2>天津时时彩</h2>
                    <van-button plain>XX分钟一期</van-button>
                    <img alt="user_avatar" src='@/assets/home/十分快三.png'>
                  </div>
                </template>
              </van-grid-item>
              <van-grid-item text class="block4">
                <template #text>
                  <p>
                    天津时时彩
                  </p>
                  <div>
                    <h2>天津时时彩</h2>
                    <van-button plain>XX分钟一期</van-button>
                    <img alt="user_avatar" src='@/assets/home/湖北快三.png'>
                  </div>
                </template>
              </van-grid-item>
              <van-grid-item text class="block5">
                <template #text>
                  <p>
                    天津时时彩
                  </p>
                  <div>
                    <h2>天津时时彩</h2>
                    <van-button plain>XX分钟一期</van-button>
                    <img alt="user_avatar" src='@/assets/home/天津时时彩.png'>
                  </div>
                </template>
              </van-grid-item>
              <van-grid-item text class="block6">
                <template #text>
                  <p>
                    天津时时彩
                  </p>
                  <div>
                    <h2>天津时时彩</h2>
                    <van-button plain>XX分钟一期</van-button>
                    <img alt="user_avatar" src='@/assets/home/一分11选5.png'>
                  </div>
                </template>
              </van-grid-item>
            </van-grid>
        </div>
      </template>
    </van-tree-select>
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
       active: 0,
      items: [{ text: '体育 ', className: 'grup1'}, { text: '真人', className: 'grup2'},{ text: '电竞', className: 'grup3'},{ text: '彩票', className: 'grup4'},{ text: '棋牌', className: 'grup5'}],
    }
  }
}
</script>
<style>
  .van-sidebar-item--select .van-sidebar-item__text {
    background-image: url('../assets/home/Untitled-1.png'); 
    
}
.content_header{
  text-align: left;
    background-size: contain;
    margin: 0 10px;
    border-radius: 9px;
    text-align: left;
    background-size: contain;
    margin: 0 10px;
    border-radius: 9px;
    box-shadow: 9px 6px 26px 6px #d7d7d7;
    /* padding: 10px; */
    padding-right: 98px;
    position: relative;
    margin-top: 10px;
  background-image: url('../assets/home/background.png');
}
.grup1 .van-sidebar-item__text::before{
  background-image: url('../assets/home/right_icon1.png'); 
}
.grup2 .van-sidebar-item__text::before{
  background-image: url('../assets/home/right_icon2.png'); 
}
.grup3 .van-sidebar-item__text::before{
  background-image: url('../assets/home/right_icon3.png'); 
}
.grup4 .van-sidebar-item__text::before{
  background-image: url('../assets/home/right_icon4.png'); 
}
.grup5 .van-sidebar-item__text::before{
  background-image: url('../assets/home/right_icon5.png'); 
}
.van-sidebar-item--select::before{
  display: none;
}
.van-sidebar-item__text {
    background: url('../assets/home/backGround_noActive_right.png'); 
    background-size: 80px 80px;
    background-position: left top;
    width: 80px;
    margin: 10px;
    background-repeat: no-repeat;
    padding-top: 45px;
    padding-bottom: 20px;
    margin-bottom: 0;
    margin-top: 3px;
}

.van-sidebar-item--select, .van-sidebar-item--select:active {
    color: #fff!important;
}
.van-sidebar-item {
    padding: 0;
    color: #a7b1b7;
    background: #fff;
}
.van-sidebar-item .van-sidebar-item__text::before {
    content: '';
    position: absolute;
    width: 30px;
    height: 30px;
    top: 9px;
    background-position: center;
    background-size: 100%;
}
.van-sidebar-item__text:before {}

.van-sidebar-item .van-sidebar-item__text::before {content: '';position: absolute;width: 30px;height: 30px;top: 9px;background-position: center;background-size: 100%;}

.content_home_grup {}


.content_home_grup .van-grid-item__content p {
    position: relative;
    width: 100%;
    display: block;
    margin-top: 0;
    margin-bottom: 0;
}
.van-tree-select__content {
    background: #f4f7f9;
}
.content_home_grup .van-grid-item__content>div {
    display: block;
    width: 100%;
    padding-left: 13px;
}
.content_home_grup .van-grid-item__content>div h2 {
    margin-bottom: 0;
    margin-top: 9px;
}
.content_home_grup .van-grid-item__content>div button.van-button {
    padding: 5px;
    height: initial;
    border-radius: 13px;
    background: rgba(255,255,255,.6);
    border: none;
}
.content_home_grup .van-grid-item__content p {
    position: relative;
    width: 100%;
    display: block;
}

.content_home_grup .van-grid-item__content>div {
    display: block;
    width: 100%;
}
.block1.van-grid-item>div {
  background-image: url('../assets/home/back1.png'); 
}
.block2.van-grid-item>div {
  background-image: url('../assets/home/back2.png'); 
}
.block3.van-grid-item>div {
  background-image: url('../assets/home/back3.png'); 
}
.block4.van-grid-item.van-grid-item>div {
  background-image: url('../assets/home/back4.png'); 
}
.block5.van-grid-item>div {
  background-image: url('../assets/home/back5.png'); 
}
.block6.van-grid-item>div {
  background-image: url('../assets/home/back6.png'); 
}
.content_home_grup .van-grid-item__content {
    /* background: red; */
    color: #fff;
    display: block;
    text-align: left;
    min-width: 200px;
    background-repeat: no-repeat;
    background-size: 100%;
    padding-bottom: 9px;
    height: auto;
    padding: 12px;
    padding-right: 60px;
    border-radius: 11px;
    margin-top: 10px;
}
.content_home_grup .van-grid-item__content>div img {
    width: 56px;
    position: absolute;
    bottom: 10px;
    right: 10px;
}
.content_home_grup .van-grid-item__content p {
    position: relative;
    width: 100%;
    display: block;
    font-size: 8pt;
}
.content_home_grup .van-grid-item__content>div h2 {
    margin-bottom: 0;
    margin-top: 9px;
    font-size: 11pt;
}
.content_home_grup .van-grid-item__content>div img {
    width: 56px;
    position: absolute;
    bottom: 10px;
    right: 10px;
}

.van-tree-select__content {
    background: #f4f7f9;
}

.content_home_grup .van-grid-item__content {
}

.content_header img {
    position: absolute;
    top: -8px;
    width: 99px;
    right: 0;
}

.content_header h2 {
    font-size: 10pt;
    padding: 10px;
    height: initial;
    padding-bottom: 0;
    margin: 0;
}

.content_header p {
    margin: 0;
    font-size: 7pt;
    padding-left: 10px;
    text-transform: uppercase;
    color: #767676;
}

.content_header button.van-button {
    padding: 8px 14px;
    height: initial;
    margin: 14px;
    margin-bottom: 9px;
    border-radius: 16px;
    background-image: url('../assets/home/button.png');
    background-size: cover;
    color: #fff;
}
</style>
