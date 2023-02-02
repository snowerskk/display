<template>
  <div class="text" :style="{ backgroundColor: color }">{{ props.text }}</div>
</template>

<script setup lang="ts">
import { ref } from 'vue'

const props = defineProps({
  text: String
})

let color = ref<string>('')

const colors = [
  'rgb(0, 199, 140, 0.8)',
  'rgb(51, 161, 201, 0.8)',
  'rgb(3, 168, 158, 0.8)',
  'rgb(255, 99, 71, 0.8)',
  'rgb(255, 127, 80, 0.8)',
  'rgb(255, 97, 0, 0.8)',
  'rgb(106, 90, 205, 0.8)',
  'rgb(128, 42, 42, 0.8)',
  'rgb(218, 112, 214, 0.8)',
  'rgb(176, 48, 96, 0.8)'
]

const setColor = () => {
  const n = parseInt(String(Math.random() * colors.length))
  color.value = colors[n]
}
setColor()
</script>

<style scoped>
.text {
  padding: 5px;
  border-radius: 6px;
  margin: 30px 0;
  color: #fff;
  font-size: 24px;
  box-shadow: 4px 4px 4px rgba(0, 0, 0, 0.6);
}
</style>
