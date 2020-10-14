<template>
  <van-nav-bar :title="msg" left-text left-arrow class="header_blue" :fixed="fixed" :class="{ HomePage: HomePage }"> 
    <template  #left>
      <van-icon v-if="!back" name="more" dot />
      <van-icon v-if="back" name="arrow-left" @click="onClickLeft" />
    </template>
    <template #right >
      <p class="infoLogin">test001 <br> <span>¥1,000,000元</span></p>
      <van-icon v-if="!back" :name="iconRight" />
    </template>
  </van-nav-bar>
</template>
<script>

export default {
  name: 'Header',
  props: {
    msg: String,
    iconRight:{
      type:String,
      default:'ellipsis'
    },
    back:{
      type:Boolean,
      default:false
    },
    HomePage:{
      type:Boolean,
      default:false
    }
  },
   data() {
    return {
      fixed:true,
    }
  },
  methods: {
    onClickLeft() {
      window.history.back();
    }
    
  },
}
</script>