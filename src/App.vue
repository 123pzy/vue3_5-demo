<template>
  测试useTemplateRef：
  <UseTemplateRef />
  <hr />
  测试Props解构：
  <Props :count="count" :msg="msg" />
  <button @click="count++">count++</button>
  <hr />
  测试useId：
  <UseId />
</template>

<script setup>
import { ref } from "vue";
import UseTemplateRef from "./components/UseTemplateRef.vue";
import Props from "./components/Props.vue";
import UseId from "./components/UseId.vue";
const count = ref(0),
  msg = ref("你好！Vue3.5！");
</script>

<style scoped>
</style>