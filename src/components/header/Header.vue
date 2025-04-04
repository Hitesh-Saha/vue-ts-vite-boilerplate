<template>
  <div class="flex gap-5 justify-center w-full items-center text-center pb-5" >
    <a href="https://vuejs.org/" target="_blank">
      <img :src="vueLogo" class="logo vue" alt="Vue logo" />
    </a>
    <h4>Vue Header</h4>
  </div>
</template>

<script setup lang="ts">
import vueLogo from '../../assets/vue.svg'
</script>

<style scoped></style>
