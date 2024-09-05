<template>
  <div>count-{{ count }}</div>
  <div>msg-{{ msg }}</div>
</template>

<script lang='ts' setup>
interface Props {
  count?: number;
  msg?: string;
}
// 解构
const { count = 0, msg = "hello vue3.5!" } = defineProps<Props>();
</script>

<style scoped>
</style>