<template>
  <div class="page">
    <Title title="配置表单" />
    <div class="content">
      <div class="block">
        由于将一部分逻辑转移到了业务中台，所以配置表单占了一部分的工作量
      </div>
    </div>
  </div>
</template>

<script setup lang="ts">
import { ref } from 'vue'
import Title from './Title.vue'

const projects = ref(['1.3版本', '1.5版本', '东海县投资评审', '国库项目pc端', '国库项目移动端', '浙江公路水运项目'])
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
</style>
