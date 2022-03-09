<template>
  <HeaderComponent />
  <HomeVue />
  <ContentVue />
  <ContactVue />
</template>

<script setup>
import HeaderComponent from './components/Header.vue'
import HomeVue from './components/Home.vue'
import ContentVue from './components/Content.vue'
import ContactVue from './components/Contact.vue'

</script>

<style lang="postcss">
@tailwind base;
@tailwind components;
@tailwind utilities;

#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
}
</style>
