<template>
  <div class="home">
    <Header msg="手机号码" :back="back"/>
    <van-cell center  title="手机号码" label="请输入手机号码" class="top_user">
    </van-cell>
    <van-cell center title="手机验证码" label="请输入手机验证码" class="top_user" >
            
        </van-cell>
    <van-row>
        <van-col offset="16" span="8">
                <van-button type="primary" class="button_submit">获取验证码</van-button>
        </van-col>
    </van-row>
    <van-cell center  title class="footer_condition">
        <template #title>
            <p>为了您的信息安全，信息在确认后将无法修改 如需帮助，请 <span>联系客服</span></p>
        </template>
    </van-cell>
  </div>
</template>

<script>
// @ is an alias to /src
import Header from '@/components/Header.vue'
export default {
  name: 'PhoneNumber',
  components: {
    Header
  },
  data() {
    return {
      back:true,
    }
  }
}
</script>
