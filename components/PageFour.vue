<template>
  <BasePage title="国库项目pc端" :left="left" left-title="主要内容" :right="[]" />
</template>

<script setup lang="ts">
import BasePage from './BasePage.vue'

const left = [
  '用户管理授权功能',
  '用户信息增加银行信息表格',
  '医药费报销标准',
  '职工子女管理',
  '签章功能',
  '新增一版差旅报销',
  '业务表单（职工医药费、子女医药费、子女医保费、保育费、通用报销、会议报销、公务接待报销、培训报销）'
]

</script>
