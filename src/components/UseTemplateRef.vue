<template>
  <span ref="spanRef">spanRef实例已打印在控制台</span>
</template>

<script lang="ts" setup>
import { useTemplateRef, nextTick } from "vue";

const spanRef = useTemplateRef("spanRef");
(async () => {
  await nextTick();
  console.log("spanRef", spanRef.value);
})();
</script>

<style scoped>
</style>