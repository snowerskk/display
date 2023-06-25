<template>
  <BasePage title="1.3版本" :left="left" :right="right" />
</template>

<script setup lang="ts">
import BasePage from './BasePage.vue'

const left = [
  '指标增加金额等筛选条件',
  '部门换接口',
  '银行信息和支付明细增加财政所号',
  '增加bak文件导出',
  '差旅报销公杂费计算天数调整',
  '增加自定义确认弹框',
  '差旅报销补助，天数增加可编辑控件，金额随天数变动'
]

const right = ['优化申请单支付明细提交校验', '修复金额精度问题', '修复指标选择bug', '发票金额类型bug']
</script>
