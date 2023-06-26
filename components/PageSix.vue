<template>
  <BasePage
    title="浙江公路水运项目"
    :left="left"
    left-title="主要内容"
    :right="right"
  />
</template>

<script setup lang="ts">
import BasePage from './BasePage.vue'

const left = ['重写支付模块', '修改指标模块']

const right = []
</script>
