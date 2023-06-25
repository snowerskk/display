<template>
  <BasePage title="1.5版本" :left="left" :right="right" />
</template>

<script setup lang="ts">
import BasePage from './BasePage.vue'

const left = [
  '根据所选部门筛选出部门下的指标和申请',
  '部门前增加单位字段',
  '公务接待报销增加人员明细导入',
  '项目库项目申报增加权限分配',
  '项目字典增加权限分配及查看详情功能',
  '保证金报销分页加字段加查询条件',
  '指标模块调整接口、增加字段'
]

const right = ['调整报销校验逻辑', '调整指标模块提交逻辑', '修复导入组件预览表格赋值bug']
</script>
