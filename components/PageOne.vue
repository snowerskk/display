<template>
  <div class="page">
    <Title :title="props.title" />
    <div class="content">
      <div class="block">
        <h3 v-click="1">主要项目及版本</h3>
        <ol class="list" v-click="2">
          <li class="item" v-for="item in projects">{{ item }}</li>
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

const projects = ref(['1.3娄葑','1.5低代码','东台自规局项目','东海县投资评审'])
</script>

<style scoped>
.page {
  background: rgba(255, 255, 255, 0.9);
  border-radius: 5px;
}
.title {
  margin-bottom: 1rem;
  margin-left: -0.05em;
  font-size: 2.25rem;
  line-height: 2.5rem;
  text-align: center;
  color: black;
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
