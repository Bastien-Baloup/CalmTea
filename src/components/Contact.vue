<template>
  <div
    id="contact"
    class="flex flex-col lg:flex-row justify-evenly w-full bg-peppermint text-castro scroll-mt-20 py-5 items-center lg:h-max rounded-t-xl drop-shadow-xl"
  >
    <section
      class="w-full lg:w-1/2 px-5 mb-5 lg:flex lg:flex-col lg:h-full lg:text-2xl lg:mb-40 max-w-2xl"
    >
      <h2
        class="text-2xl underline text-center mb-5 lg:text-3xl lg:mb-20 lg:mt-20"
      >Sign up to our newsletter</h2>
      <form @submit.prevent>
        <div class="flex mb-2 border-castro border-b-2 border-opacity-50">
          <label class="w-1/3 block" for="email">Email&nbsp;:</label>
          <input
            id="email"
            class="w-2/3 block bg-beige rounded-sm focus:outline-castro px-1"
            type="email"
            name="email"
          />
        </div>
        <input
          class="ml-auto block border-2 border-castro rounded-md p-1 hover:bg-beige active:bg-castro active:text-beige"
          type="submit"
          value="Sign up"
        />
      </form>
    </section>
    <section
      class="w-full lg:w-1/2 px-5 lg:flex lg:flex-col lg:h-full lg:text-2xl lg:mb-20 max-w-2xl"
    >
      <h2 class="text-2xl underline text-center mb-5 lg:text-3xl lg:mb-20 lg:mt-20">Contact us</h2>
      <form @submit.prevent>
        <div class="flex mb-2 border-castro border-b-2 border-opacity-50">
          <label class="w-1/3 block" for="contact-email">Email&nbsp;:</label>
          <input
            id="contact-email"
            class="w-2/3 block bg-beige rounded-sm focus:outline-castro px-1"
            type="contact-email"
            name="contact-email"
          />
        </div>
        <div class="flex mb-2 border-castro border-b-2 border-opacity-50">
          <label class="w-1/3 block" for="message">Message&nbsp;:</label>
          <textarea
            id="message"
            class="w-2/3 block bg-beige rounded-sm focus:outline-castro px-1"
            name="message"
          />
        </div>

        <input
          class="ml-auto block border-2 border-castro rounded-md p-1 hover:bg-beige active:bg-castro active:text-beige"
          type="submit"
          value="Send"
        />
      </form>
    </section>
  </div>
</template>
