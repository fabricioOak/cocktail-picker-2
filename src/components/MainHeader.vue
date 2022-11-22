<template>
  <header class="w-full px-8 text-gray-700 bg-white shadow-md">
    <div
      class="container flex flex-col flex-wrap items-center justify-between py-5 mx-auto md:flex-row max-w-7xl"
    >
      <div class="relative items-center flex flex-col md:flex-row">
        <img class="h-12" src="../assets/images/logo.svg" alt="Site logo" />
        <router-link
          :to="{ path: '/' }"
          class="flex items-center mb-5 font-medium text-gray-900 lg:w-auto lg:items-center lg:justify-center md:mb-0"
        >
          <span
            class="mx-auto mt-2 text-xl font-black leading-none text-gray-900 select-none"
            >Cocktail Picker<span class="text-pink-600">.</span></span
          >
        </router-link>
      </div>
      <div class="relative">
        <label for="SearchBar" class="sr-only"> Email </label>
        <input
          type="text"
          id="SearchBar"
          placeholder="Search here"
          class="outline-none focus:border-b-8 w-80 rounded-md p-2.5 pr-10 sm:text-sm focus:outline-none border-b-2 duration-300"
        />
        <span class="absolute inset-y-0 right-0 grid w-10 place-content-center">
          <button
            type="button"
            class="rounded-full bg-pink-600 p-0.5 text-white hover:bg-pink-700"
          >
            <svg
              class="h-6 w-6 p-1 invert"
              xmlns="http://www.w3.org/2000/svg"
              viewBox="0 0 512 512"
            >
              <path
                d="M416 208c0 45.9-14.9 88.3-40 122.7L502.6 457.4c12.5 12.5 12.5 32.8 0 45.3s-32.8 12.5-45.3 0L330.7 376c-34.4 25.2-76.8 40-122.7 40C93.1 416 0 322.9 0 208S93.1 0 208 0S416 93.1 416 208zM208 352c79.5 0 144-64.5 144-144s-64.5-144-144-144S64 128.5 64 208s64.5 144 144 144z"
              />
            </svg>
          </button>
        </span>
      </div>
    </div>
  </header>
</template>

<script setup>
defineProps({
  drink: String,
});
defineEmits(["input", "search-drink"]);
</script>

<style></style>
