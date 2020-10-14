<template>
  <div class="home">
    <Header msg="个人资料" back="true"/>
    <van-cell center  title="我的头像" class="top_user info">
    </van-cell>
    <van-cell center  title icon class="top_user" @click="show = true">
      <template #right-icon>
      </template>
       <template #icon>
        <img alt="user_avatar" src="../assets/user/icone_top_edit.png">
      </template>
    </van-cell>
    <van-cell center  title="用户名" label="test001" class="top_user info">
    </van-cell>
    <van-cell-group class="link_user info">
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
    <van-cell center  title class="footer_condition">
        <template #title>
            <p>为了您的心思安全，信息在确认后将无法修改 如需帮助，请 <span>联系客服</span></p>
        </template>
    </van-cell>
    <van-action-sheet v-model="show" @cancel="onCancel"  cancel-text="取消">
        <div class="content">
            <van-grid :border="false" :column-num="4">
                <van-grid-item v-for="image in images" :key="image">
                    <img alt=""  :src="image.name" class="profil_user"/>
                </van-grid-item>
            </van-grid>
            <van-cell-group>
                <van-cell title="从相册选取"  />
                <van-cell title="拍照"  />
            </van-cell-group>
        </div>
    </van-action-sheet>
  </div>
</template>

<script>
// @ is an alias to /src
import Header from '@/components/Header.vue'
import { Toast } from 'vant';
export default {
  name: 'DetailUser',
   data() {
    return {
      show: false,
      images: [
        { name: require('@/assets/user/person1.png') },
        { name: require('@/assets/user/person2.png') },
        { name: require('@/assets/user/person3.png') },
        { name: require('@/assets/user/person4.png') },
        { name: require('@/assets/user/person5.png') },
        { name: require('@/assets/user/person6.png') },
        { name: require('@/assets/user/person7.png') },
        { name: require('@/assets/user/person8.png') },
      ],
    };
  },
  components: {
    Header
  },
  methods: {
    onCancel() {
      Toast('cancel');
    },
  },
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
</style>