<template>
  <view class="content">
    <image class="logo" src="/static/logo.png" />
    <view class="text-area">
      <text class="title">{{ title }}</text>
    </view>
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
const title = ref("login");
const getPhoneNumber = (e) => {
  const { code } = e.detail;
  console.log("number", code);
};
</script>

<style>
.content {
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

.text-area {
  display: flex;
  justify-content: center;
}

.title {
  font-size: 36rpx;
  color: #8f8f94;
}
</style>
