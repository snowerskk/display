<template>
  <div class="page">
    <Title :title="props.title" />
    <div class="content">
      <div class="block">
        <ul class="list" v-click="1">
          <li class="item" v-for="item in modules">{{ item }}</li>
        </ul>
      </div>
    </div>
  </div>
</template>

<script setup lang="ts">
import { ref } from 'vue'
import Title from './Title.vue'

const props = defineProps({
  title: String
})

const modules = ref([
  '一级指标编制',
  '二级指标编制',
  '指标调整单',
  '指标调剂单',
  '指标冻结',
  '指标解冻',
  '通用报销',
  '公务接待报销',
  '会议报销',
  '培训报销',
  '差旅报销',
  '合同报销',
  '公务用车报销',
  '保证金报销',
  '借款单',
  '还款单',
  '项目申报',
  '项目储备',
  '项目结项',
  '项目申报',
  '项目总览',
  '参评单位',
  '协审单位抽签',
  '审核报告',
  '统计',
  '费用结算',
  '支付申请单',
  '支付进度登记簿'
])
</script>

<style scoped>
.page {
  background: rgba(255, 255, 255, 0.9);
  border-radius: 5px;
}
.content {
  color: #000;
}
.block {
  background: #fff;
}
.list {
  list-style: none;
  display: flex;
  flex-wrap: wrap;
  justify-content: flex-start;
}
.item {
  flex-grow: 1;
  width: 20%;
  background: snow;
  border-bottom: 1px dashed #eee;
}
</style>
