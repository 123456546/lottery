<template>
  <div class="home">
    <Header msg="个人资料" :back="back"/>
    <van-cell center  title="我的头像" class="top_user info">
    </van-cell>
    <van-cell center  title icon class="top_user" @click="show = true">
      <template #right-icon>
      </template>
       <template #icon>
        <img alt="user_avatar" src="@/assets/user/icone_top_edit.png">
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
        <van-cell center title="手机号码" label="绑定手机号码以保护账号安全" is-link to="PhoneNumber" >
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
                <van-grid-item v-for="(image,key) in images" :key="key">
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
      back:true,
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
