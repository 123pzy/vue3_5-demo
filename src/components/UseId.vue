<template>
  <from>
    <label :for="id">Name:</label>
    <input type="text" :id="id" />
  </from>
</template>

<script lang='ts' setup>
import { useId } from "vue";

const id = useId();
</script>

<style scoped>
</style>