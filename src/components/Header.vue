<template>
  <van-nav-bar :title="msg" left-text left-arrow class="header_blue" fixed="true"> 
    <template  #left>
      <van-icon v-if="!back" name="more" dot />
      <van-icon v-if="back" name="arrow-left" @click="onClickLeft" />
    </template>
    <template #right>
      <van-icon v-if="!back"  name="setting-o" />
    </template>
  </van-nav-bar>
</template>
<script>

export default {
  name: 'Header',
  props: {
    msg: String,
    back:{
      type:Boolean,
      default:false
    }
  },
  methods: {
    onClickLeft() {
      window.history.back();
    }
    
  },
}
</script>
<style>
  .header_blue{
      background-image: linear-gradient(to right, #3570f7 , #2797ff);

  }
  .header_blue .van-icon {
    color: #fff!important;
    font-size: 16pt;
  }

  .header_blue .van-nav-bar__title {
      color: #fff;
      font-size: 17pt;
  }
</style>