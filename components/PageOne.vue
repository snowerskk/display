<template>
  <div class="page">
    <Title title="2023上半年工作总结" />
    <div class="content">
      <div class="block">
        <ol class="list" v-click="1">
          <li class="item" v-for="item in projects">💠{{ item }}</li>
        </ol>
      </div>
    </div>
  </div>
</template>

<script setup lang="ts">
import { ref } from 'vue'
import Title from './Title.vue'

const projects = ref(['1.3版本', '1.5版本', '东海县投资评审', '国库项目pc端', '国库项目移动端', '浙江交科院项目'])
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
  padding-bottom: 20px;
}
.item {
  border-bottom: 1px solid #eee;
}
</style>
