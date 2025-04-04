<template>
  <div class="flex gap-5 justify-center w-full items-center">
    <a href="https://vitejs.dev" target="_blank">
      <img src="/vite.svg" class="logo" alt="Vite logo" />
    </a>
    <a href="https://vuejs.org/" target="_blank">
      <img :src="vueLogo" class="logo vue" alt="Vue logo" />
    </a>
  </div>
  <Counter title="Hello World!!" />
</template>

<script setup lang="ts">
import Counter from "../../components/counter/Counter.vue";
import vueLogo from "../../assets/vue.svg";
</script>

<style scoped></style>
