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
  '金额区间选择器',
  '树形选择器（单选部分）',
  '懒加载列表',
  '选择器头部组件',
  '筛选条件表单',
  '结算方式',
  '表单渲染组件',
  '分页渲染组件'
]

const right = [
  '工作台',
  '待办列表',
  '代办页筛选',
  '交通费卡片',
  '住宿费卡片',
  '补助卡片',
  '业务表单（职工医药费、子女医药费、子女医保费、保育费、通用报销、会议报销、公务接待报销、培训报销）'
]
</script>
