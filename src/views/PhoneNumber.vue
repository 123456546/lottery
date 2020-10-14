<template>
  <div class="home">
    <Header msg="手机号码" back="true"/>
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
            <p>为了您的心思安全，信息在确认后将无法修改 如需帮助，请 <span>联系客服</span></p>
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
    padding-top: 50px;
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
.top_user.info {
    padding: 0;
}

.top_user.info .van-cell__title,.link_user.info .van-cell__title {
    padding-left: 9px;
}


.link_user.info .van-cell {
    padding-left: 0;
}

.link_user.info {
    padding-top: 0;
    padding-bottom: 0;
}
.footer_condition {background: #f2f4f8;color: #a1a3a6;font-size: 10pt;}

.footer_condition p span {
    color: #6091ff;
}
img.profil_user {
    width: 60px;
}

button.button_submit.van-button {
    padding: 6px 9px;
    height: initial;
    margin-bottom: 11px;
    background: #f2d6b6;
    border-color: #f2d6b6;
    font-weight: 500;
}
</style>