<template>
  <HeaderComponent />
  <HomeVue />
  <ContentVue />
  <ContactVue />
  <FooterVue />
</template>

<script setup>
import HeaderComponent from './components/Header.vue'
import HomeVue from './components/Home.vue'
import ContentVue from './components/Content.vue'
import ContactVue from './components/Contact.vue'
import FooterVue from './components/Footer.vue'

</script>

<style lang="postcss">
@tailwind base;
@tailwind components;
@tailwind utilities;

#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  @apply bg-beige overflow-x-hidden scroll-smooth antialiased;
}
</style>
