<template>
  <h1 class="text-center">{{ props.title }}</h1>

  <div class="card flex flex-col gap-3 justify-center items-center">
    <div class="card-body">
      <h5 class="card-title text-3xl">{{ counter.count }}</h5>
    </div>
    <div class="flex gap-5">
      <button type="button" @click="counter.increment">Increment</button>
      <button type="button" @click="counter.decrement">Decrement</button>
    </div>
    <div class="text-2xl">Double count is {{ counter.doubleCount }}</div>
    <div class="flex gap-5">
      <button type="button" @click="counter.reset">Reset</button>
    </div>

  </div>

  <p class="text-center">
    Check out
    <a href="https://vuejs.org/guide/quick-start.html#local" target="_blank"
      >create-vue</a
    >, the official Vue + Vite starter
  </p>
  <p class="text-center">
    Install
    <a href="https://github.com/vuejs/language-tools" target="_blank">Volar</a>
    in your IDE for a better DX
  </p>
  <p class="read-the-docs text-center">Click on the Vite and Vue logos to learn more</p>
</template>

<script setup lang="ts">
import { useCounterStore } from '../../store/counter'

const props = defineProps({
  title: {
    type: String,
  }
})

const counter = useCounterStore()
</script>

<style scoped>
.read-the-docs {
  color: #888;
}
</style>
