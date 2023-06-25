<template>
  <div class="page">
    <Title :title="props.title" />
    <div class="content">
      <div class="block">
        <Card :title="leftTitle" v-click="1" v-if="left.length">
          <ol>
            <li v-for="row of left">{{ row }}</li>
          </ol>
        </Card>
        <Card :title="rightTitle" v-click="2" v-if="right.length">
          <ol>
            <li v-for="row of right">{{ row }}</li>
          </ol>
        </Card>
      </div>
    </div>
  </div>
</template>

<script setup lang="ts">
import { type PropType } from 'vue'
import Title from './Title.vue'

const props = defineProps({
  title: {
    type: String,
    required: true
  },
  left: {
    type: Array as PropType<string[]>,
    required: true
  },
  leftTitle: {
    type: String,
    default: '新增需求及需求调整'
  },
  right: {
    type: Array as PropType<string[]>,
    required: true
  },
  rightTitle: {
    type: String,
    default: '优化代码及BUG修复'
  }
})
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
  display: flex;
}
.list {
  list-style: none;
}
.item {
  border-bottom: 1px solid #eee;
}
</style>
