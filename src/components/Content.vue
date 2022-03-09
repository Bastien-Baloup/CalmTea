<template>
  <div
    id="content"
    class="flex flex-col-reverse lg:flex-row justify-evenly w-full bg-beige text-castro scroll-mt-20"
  >
    <div
      class="m-auto text-xl h-max lg:w-max lg:max-h-full p-5 flex-shrink lg:overflow-auto lg:z-10 bg-transparent"
    >
      <p
        class="mb-5"
      >Calm Tea's recipe is simple. No preservatives, no colorants, only what is needed&nbsp;:</p>
      <div class="ml-5">
        <details class="cursor-pointer text-base max-w-prose lg:mb-2">
          <summary class="text-xl">White tea</summary>
          <p
            class="text-base ml-5 px-5 py-3 border-l-2 border-castro bg-peppermint bg-opacity-50"
          >With its low amount of caffeine and its high amount of L-theanine, white tea is known to help relax while also increasing focus.</p>
        </details>
        <details class="cursor-pointer text-base max-w-prose lg:mb-2">
          <summary class="text-xl">Peppermint</summary>
          <p
            class="text-base ml-5 px-5 py-3 border-l-2 border-castro bg-peppermint bg-opacity-50"
          >The menthol in peppermint can act as a muscle relaxant and pain reliever. Relieving tension being a core part of relaxing.</p>
        </details>
        <details class="cursor-pointer text-base max-w-prose lg:mb-2">
          <summary class="text-xl">Jasmine</summary>
          <p
            class="text-base ml-5 px-5 py-3 border-l-2 border-castro bg-peppermint bg-opacity-50"
          >Jasmine is known to have a calming effect on the nervous system, improving restlessness, irritability, and insomnia. Jasmine is also known to ease muscle tension.</p>
        </details>
        <details class="cursor-pointer text-base max-w-prose lg:mb-2">
          <summary class="text-xl">Chamomile</summary>
          <p
            class="text-base ml-5 px-5 py-3 border-l-2 border-castro bg-peppermint bg-opacity-50"
          >Studies have shown chamomile to be effective in aiding relaxation, and also helping with anxiety, depression, and insomnia.</p>
        </details>
        <details class="cursor-pointer text-base max-w-prose lg:mb-2">
          <summary class="text-xl">Vitamin C</summary>
          <p
            class="text-base ml-5 px-5 py-3 border-l-2 border-castro bg-peppermint bg-opacity-50"
          >Vitamin C is known to help mood and lower anxiety levels.</p>
        </details>
        <details class="cursor-pointer text-base max-w-prose lg:mb-2">
          <summary class="text-xl">Stevia</summary>
          <p
            class="text-base ml-5 px-5 py-3 border-l-2 border-castro bg-peppermint bg-opacity-50"
          >Stevia is a 100% natural sweetener with many health benefits.</p>
        </details>
      </div>
    </div>
    <img
      class="h-screen object-cover lg:h-auto lg:w-1/2 lg:-mr-20 lg:-ml-10 lg:flex-shrink"
      src="/frontAndBack.png"
      alt
    />
  </div>
</template>

<script setup>
</script>


<style lang="postcss">
@media screen(lg) {
  #content {
    height: calc(100vh - 5rem); /* viewport height - header height */
  }
}

/* set custom detail arrow */
summary {
  list-style-image: url(/chevron-right-solid.svg);
}

summary::-webkit-details-marker {
  background: url(/chevron-right-solid.svg);
  color: transparent;
}

/* change custom detail arrow when open */
details[open] summary {
  list-style-image: url(/chevron-down-solid.svg);
}

details[open] summary::-webkit-details-marker {
  background: url(/chevron-down-solid.svg);
  color: transparent;
}
</style>