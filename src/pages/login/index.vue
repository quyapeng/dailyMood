<template>
  <view class="login">
    <image class="logo" src="/static/logo.png" />
    <button
      class="btn"
      round
      size="small"
      open-type="getPhoneNumber"
      @getphonenumber="getPhoneNumber"
    >
      <i class="icon-wechat" />微信用户一键登录
    </button>
  </view>
</template>

<script setup lang="ts">
import { ref } from "vue";
const getPhoneNumber = (e) => {
  const { code } = e.detail;
  console.log("number", code);
};
</script>

<style>
.login {
  display: flex;
  flex-direction: column;
  align-items: center;
  justify-content: center;
}

.logo {
  height: 200rpx;
  width: 200rpx;
  margin-top: 200rpx;
  margin-left: auto;
  margin-right: auto;
  margin-bottom: 50rpx;
}
</style>
