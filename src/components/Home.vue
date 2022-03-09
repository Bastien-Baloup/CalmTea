<template>
  <!-- hero -->
  <div id="hero" class="w-full mt-20 bg-beige scroll-mt-20">
    <img class="h-full w-auto max-w-full m-auto max-w-screen object-cover" src="/pattern.png" alt />
  </div>
  <!-- home section -->
  <section
    id="home"
    class="flex flex-col items-center justify-evenly w-full bg-peppermint scroll-mt-20"
  >
    <img class="w-1/2" src="/logo-textless_castro.png" alt />
    <p class="text-castro text-2xl text-center px-10">
      <strong class="font-bold text-3xl">Calm Tea</strong> is a fresh beverage specialy crafted for a relaxing moment.
      <br />Simply open the can, lay back, and enjoy the taste of white tea, peppermint, jasmine and chamomile.
    </p>
  </section>
</template>

<script setup>
</script>

<style lang="postcss">
#hero,
#home {
  height: calc(100vh - 5rem); /* viewport height - header height */
}
</style>