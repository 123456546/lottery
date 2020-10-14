<template>
  <div class="home">
    <Header msg="个人资料" back="true"/>
    <van-cell center  title="我的头像" class="top_user">
    </van-cell>
    <van-cell center  title icon class="top_user">
      <template #right-icon>
      </template>
       <template #icon>
        <img alt="user_avatar" src="../assets/user/icone_top_edit.png">
      </template>
    </van-cell>
    <van-cell center  title="用户名" label="test001" class="top_user">
    </van-cell>
    <van-cell-group class="link_user">
        <van-cell center title="真实姓名" label="真实姓名需与银行卡持卡人姓名一致，否则无法提款" >
            <template #right-icon>
            <van-icon name="arrow" class="arrow" />
            </template>
        </van-cell>
        <van-cell center title="性别" label="请选择您的性别" >
            <template #right-icon>
            <van-icon name="arrow" class="arrow" />
            </template>
        </van-cell>
        <van-cell center title="出生日期" label="添加日期，以确保您已满18周岁" >
            <template #right-icon>
            <van-icon name="arrow" class="arrow" />
            </template>
        </van-cell>
        <van-cell center title="手机号码" label="绑定手机号码以保护账号安全" >
            <template #right-icon>
            <van-icon name="arrow" class="arrow" />
            </template>
        </van-cell>
        <van-cell center title="趣聊号" label="绑定趣聊号以保护账号安全" >
            <template #right-icon>
            <van-icon name="arrow" class="arrow" />
            </template>
        </van-cell>
        <van-cell center title="电子邮箱" label="绑定邮箱以保护账号安全" >
            <template #right-icon>
            <van-icon name="arrow" class="arrow" />
            </template>
        </van-cell>
      
    </van-cell-group>
  </div>
</template>

<script>
// @ is an alias to /src
import Header from '@/components/Header.vue'

export default {
  name: 'DetailUser',
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
</style>