<template>
  <van-nav-bar :title="msg" left-text left-arrow class="header_blue" :fixed="fixed"> 
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