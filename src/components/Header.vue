<template>
  <!-- larger header with visible nav -->
  <header class="h-20 w-full bg-peppermint fixed top-0 z-20 hidden lg:flex rounded-b-xl">
    <nav class="flex w-full">
      <a href="#hero" class="m-auto" @click="closeMenu">
        <img src="/logo_castro.png" alt class="h-12" />
      </a>
      <a
        class="text-castro text-xl font-bold hover:underline m-auto"
        href="#home"
        @click="closeMenu"
      >Home</a>
      <a
        class="text-castro text-xl font-bold hover:underline m-auto"
        href="#content"
        @click="closeMenu"
      >Content</a>

      <a
        class="text-castro text-xl font-bold hover:underline m-auto"
        href="#contact"
        @click="closeMenu"
      >Contact</a>
    </nav>
  </header>
  <!-- small screen header with burger menu -->
  <header class="flex h-20 w-full bg-peppermint fixed top-0 z-20 lg:hidden rounded-b-xl">
    <button
      class="my-auto mx-4 fill-castro p-1 outline-none focus:outline-castro hover:outline-castro rounded"
      aria-label="menu"
      @click="openMenu"
    >
      <svg class="w-6 h-6" version="1.1" viewBox="0 0 270792 249118">
        <path d="M0 0h270792v42287H0zm0 103118h270792v42287H0zm0 103716h270792v42283H0" />
      </svg>
    </button>
    <a
      href="#hero"
      class="absolute top-1/2 left-1/2 transform -translate-x-1/2 -translate-y-1/2"
      @click="closeMenu"
    >
      <img src="/logo_castro.png" alt class="h-12" />
    </a>
    <nav
      class="absolute top-20 w-screen bg-beige transition-all duration-300 h-auto overflow-hidden"
      :class="menuIsOpen ? 'max-h-screen' : 'max-h-0'"
    >
      <ul>
        <li>
          <a
            class="text-castro text-lg hover:underline border-castro border-b-2 border-opacity-50 w-screen block"
            href="#home"
            @click="closeMenu"
          >Home</a>
        </li>
        <li>
          <a
            class="text-castro text-lg hover:underline border-castro border-b-2 border-opacity-50 w-screen block"
            href="#content"
            @click="closeMenu"
          >Content</a>
        </li>
        <li>
          <a
            class="text-castro text-lg hover:underline border-castro border-b-2 border-opacity-50 w-screen block"
            href="#contact"
            @click="closeMenu"
          >Contact</a>
        </li>
      </ul>
    </nav>
    <div
      v-if="menuIsOpen"
      class="h-full w-full -z-10 fixed bg-opacity-5 bg-black"
      @click="closeMenu"
    />
  </header>
</template>

<script setup>
import { ref } from 'vue'

const menuIsOpen = ref(false)
const openMenu = () => menuIsOpen.value = true
const closeMenu = () => menuIsOpen.value = false

</script>