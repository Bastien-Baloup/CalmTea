<template>
  <HeaderComponent />
</template>

<script setup>
import HeaderComponent from './components/Header.vue'

</script>

<style lang="postcss">
@tailwind base;
@tailwind components;
@tailwind utilities;

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
