<template>
  <view class="index">
    <view class="item">
      <i></i>
      <h3>早起</h3>
      <view>
        <h4>10</h4>
        <p>坚持天数</p>
      </view>
    </view>
  </view>
</template>

<script setup lang="ts">
import { ref } from "vue";
const title = ref("index");
</script>

<style>
.index {
  display: flex;
  flex-direction: column;
  align-items: center;
  justify-content: center;
}
</style>
