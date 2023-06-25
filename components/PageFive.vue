<template>
  <BasePage
    title="国库项目移动端"
    :left="left"
    left-title="基础组件"
    :right="right"
    right-title="主要业务"
  />
</template>

<script setup lang="ts">
import BasePage from './BasePage.vue'

const left = [
  '附件',
  '审批',
  '卡片按钮',
  '新增按钮',
  '下拉选择器',
  '弹框选择器',
  '级联选择器',
  '日期选择器',
  '树形选择器（单选部分）',
  '懒加载列表',
  '选择器头部组件',
  '筛选条件表单',
  '结算方式',
  '表单渲染组件',
  '分页渲染组件'
]

const right = []
</script>
