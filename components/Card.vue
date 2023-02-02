<template>
  <div class="card" :style="{ backgroundColor: color, width: props.width }">
    <div class="title">{{ props.title }}</div>
    <div class="content"><slot /></div>
  </div>
</template>

<script setup lang="ts">
import { ref } from 'vue'

const props = defineProps({
  title: String,
  width: {
    type: String,
    default: '42%'
  }
})

let color = ref<string>('')

const colors = [
  'rgb(0, 199, 140, 0.6)',
  'rgb(51, 161, 201, 0.6)',
  'rgb(3, 168, 158, 0.6)',
  'rgb(255, 99, 71, 0.6)',
  'rgb(255, 127, 80, 0.6)',
  'rgb(255, 97, 0, 0.6)',
  'rgb(106, 90, 205, 0.6)',
  'rgb(135, 206, 235, 0.6)',
  'rgb(128, 42, 42, 0.6)',
  'rgb(218, 112, 214, 0.6)',
  'rgb(176, 48, 96, 0.6)'
]

const setColor = () => {
  const n = parseInt(String(Math.random() * colors.length))
  color.value = colors[n]
}
setColor()
</script>

<style scoped>
.card {
  padding: 10px;
  border-radius: 6px;
  margin: 20px;
  color: #000;
  box-shadow: 4px 4px 4px rgba(0, 0, 0, 0.6);
}
.title {
  text-align: center;
  font-weight: 600;
  font-size: 20px;
  border-bottom: 2px dashed #eee;
}
.content {
  box-shadow: inset -4px -4px 10px #fff;
  padding: 4px;
}
</style>
