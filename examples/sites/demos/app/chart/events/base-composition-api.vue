<template>
  <tiny-chart-pie :data="chartData" :settings="chartSettings" :events="chartEvents" judge-width> </tiny-chart-pie>
</template>

<script setup lang="jsx">
import { ref } from 'vue'
import { ChartPie as TinyChartPie } from '@opentiny/vue'

const chartData = ref({
  columns: ['日期', '访问用户'],
  rows: [
    { 日期: '1/1', 访问用户: 1393 },
    { 日期: '1/2', 访问用户: 3530 },
    { 日期: '1/3', 访问用户: 2923 },
    { 日期: '1/4', 访问用户: 1723 },
    { 日期: '1/5', 访问用户: 3792 },
    { 日期: '1/6', 访问用户: 4593 }
  ]
})
const chartSettings = ref({
  selectedMode: 'single',
  hoverAnimation: false
})
const chartEvents = ref({
  click: (data) => {
    alert(`被点击日期：${data.name}`)
  }
})
</script>
