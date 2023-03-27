<template>
  <view class="index">
    <view class="item">
      <image
        class="img"
        mode="aspectFit"
        src="https://web-assets.dcloud.net.cn/unidoc/zh/cat-2.png"
      ></image>
      <view class="textcenter">早起</view>
      <view class="sub">
        <text>10</text>
        <p class="subtext">坚持天数</p>
      </view>
    </view>
  </view>
</template>

<script setup lang="ts">
import { ref } from "vue";
const title = ref("index");
</script>

<style>
.item {
  display: flex;
  flex-direction: row;
  align-items: center;
  justify-content: space-between;
  padding: 10px 20px;
  background-color: #2accd4;
  margin: 10px;
  border-radius: 8px;
  border: 1px solid #12898f;
}

.item .textcenter {
  flex: 1;
}
.item .img {
  width: 60px;
  height: 60px;
  background-color: #eee;
  margin-right: 10px;
}
.item .sub text {
  display: block;
  width: 100%;
  font-size: 26px;
  text-align: center;
}
.item .sub .subtext {
  font-size: 12px;
}
</style>
