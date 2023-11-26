
<script setup>
const props = defineProps({
  title: {
    type: String,
    required: false,
    default: "Hero title",
  },
  description: {
    type: String,
    required: false,
    default: "Hero description",
  },
  leftButtonText: {
    type: String,
    required: false,
    default: "Button1",
  },
  rightButtonText: {
    type: String,
    required: false,
    default: "Button2",
  },
  heroImage: {
    type: String,
    required: false,
    default: "https://dummyimage.com/720x600/edf2f7/a5afbd",
  },
});
</script>

<template>
  <section class="text-gray-700 body-font">
    <div
      class="container mx-auto flex px-5 py-24 md:flex-row flex-col items-center"
    >
      <div
        class="lg:flex-grow md:w-1/2 lg:pr-24 md:pr-16 flex flex-col md:items-start md:text-left mb-16 md:mb-0 items-center text-center"
      >
        <h1
          class="title-font sm:text-4xl text-3xl mb-4 font-medium text-gray-900"
        >
          {{ title }}
        </h1>
        <p class="mb-8 leading-relaxed">
          {{ description }}
        </p>
        <div class="flex justify-center">
          <button
            class="inline-flex text-white bg-indigo-500 border-0 py-2 px-6 focus:outline-none hover:bg-indigo-600 rounded text-lg"
          >
            {{ leftButtonText }}
          </button>
          <button
            class="ml-4 inline-flex text-gray-700 bg-gray-200 border-0 py-2 px-6 focus:outline-none hover:bg-gray-300 rounded text-lg"
          >
            {{ rightButtonText }}
          </button>
        </div>
      </div>
      <div class="lg:max-w-lg lg:w-full md:w-1/2 w-5/6">
        <img
          class="object-cover object-center rounded"
          alt="hero"
          :src="heroImage"
        />
      </div>
    </div>
  </section>
</template>


<style>
</style>