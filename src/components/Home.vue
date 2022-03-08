<template>
  <div id="hero" class="w-screen mt-20 bg-beige">
    <img class="h-full w-full max-w-screen object-cover" src="/pattern.png" alt />
  </div>
  <div id="home" class="flex flex-col items-center justify-evenly w-full bg-peppermint">
    <img class="w-1/2" src="/logo-textless_castro.png" alt />
    <p class="text-castro text-2xl text-center px-10">
      <strong class="font-bold text-3xl">Calm Tea</strong> is a fresh beverage specialy crafted for a relaxing moment.
      <br />Lorem ipsum dolor sit amet consectetur adipisicing elit. Modi laudantium quis, inventore debitis aliquam impedit neque maiores, voluptas repellendus perferendis eius provident pariatur incidunt? Mollitia sapiente quasi hic expedita eos.
    </p>
  </div>
</template>

<script setup>
</script>

<style lang="postcss">
#hero,
#home {
  height: calc(100vh - 5rem);
}
</style>