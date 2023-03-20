<template>
  <view class="me"> {{ title }}</view>
</template>

<script setup lang="ts">
import { ref } from "vue";
const title = ref("me");
</script>

<style>
.me {
  text-align: center;
}
</style>
