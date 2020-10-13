<template>
  <van-nav-bar :title="msg" left-text left-arrow class="header_blue">
    <template #left>
      <van-icon name="more" dot />
    </template>
    <template #right>
      <van-icon name="setting-o" />
    </template>
  </van-nav-bar>
</template>
<script>

export default {
  name: 'Header',
  props: {
    msg: String
  }
}
</script>
<style scoped>
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