<template>
  <div class="page">
    <Title :title="props.title" />
    <div class="content">
      <div class="block">
        <ol class="list" v-click="1">
          <li class="item" v-for="item in modules">{{ item }}</li>
        </ol>
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

const modules = ref(['指标管理','报销管理','借款管理','项目库','项目评审','支付管理'])
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
.item {
  border-bottom: 1px solid #eee;
}
</style>
