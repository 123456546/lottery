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
<style  scoped>
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
</style>