<template>
  <page-content title="Button" desc="按钮，WeUI采用小程序原生的按钮为主体，加入一些间距的样式。">
    <div class="button-content">
      <mp-button type="default" size="large" btnClass="mb15">默认按钮</mp-button>
      <mp-button type="primary" size="large" btnClass="mb15">主要按钮</mp-button>
      <mp-button type="warn" size="large" btnClass="mb15">警告按钮</mp-button>
      <mp-button type="defualt" size="normal" btnClass="mb15 mr15" plain>默认按钮</mp-button>
      <mp-button type="primary" size="normal" btnClass="mb15 mr15" plain>主要按钮</mp-button>
      <mp-button type="warn" size="normal" btnClass="mb15" plain>警告按钮</mp-button>
      <mp-button type="primary" size="normal" btnClass="mb15 mr15">普通按钮</mp-button>
      <mp-button type="primary" size="small" btnClass="mb15 mr15">小型按钮</mp-button>
      <mp-button type="primary" size="mini" btnClass="mb15">迷你按钮</mp-button>
      <mp-button type="primary" size="large" btnClass="mb15" disabled>禁用按钮</mp-button>
      <mp-button type="primary" size="large" btnClass="mb15" loading>加载按钮</mp-button>
      <mp-button type="default" size="large" btnClass="mb15" openType="getUserInfo" @getuserinfo="getuserinfo">获取用户信息</mp-button>
      <mp-button type="primary" size="large" btnClass="mb15" openType="getPhoneNumber" @getphonenumber="getphonenumber">获取手机号码</mp-button>
      <mp-button type="default" size="large" btnClass="mb15" openType="contact" sendMessagePath="/pages/index/main" showMessageCard @contact="contact" sendMessageTitle="会话卡片标题" sendMessageImg="/static/images/contact-test.jpg">显示卡片</mp-button>
    </div>
  </page-content>
</template>

<script>
import mpButton from '../../../src/button';
import pageContent from '../../components/page-content';
/* import { mpButton } from '../../../src/index.js'; */
export default {
  components: {
    mpButton,
    pageContent
  },
  methods: {
    contact(e) {
      console.log(e);
    },
    getuserinfo(e) {
      console.log(e);
    },
    getphonenumber(e) {
      console.log(e);
    }
  }
};
</script>

<style scoped>
.hover-class {
  color: aqua;
}
</style>
