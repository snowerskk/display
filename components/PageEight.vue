<template>
  <BasePage title="东海县投资评审" :left="left" left-title="需求变更" :right="[]" />
</template>

<script setup lang="ts">
import BasePage from './BasePage.vue'

const left = [
  '申请表单页面调整',
  '抽签结果页面调整',
  '核增核减率（一审）、综合误差率（二审/概算）显示调整',
  '页面增加导出功能（所有菜单页面、带筛选）'
]

</script>
