<script lang="ts" setup>
import { Icon } from '@iconify/vue'
</script>

<template>
  <main class="main pt-8">
    <div class="flex flex-col justify-center items-center text-center">
      <h1
        class="py-4 px-6 text-3xl text-transparent bg-clip-text bg-gradient-to-r from-purple-500 to-pink-500 md:text-5xl font-bold"
      >
        Welcome to my Wallet project
      </h1>
      <h2 class="py-4 px-12 text-sm md:text-xl">
        There is fullStack app which helps u to see where u spend your
        <span class="text-amber-400">gold</span> ?!
      </h2>
      <h3 class="pt-4">What does it look like</h3>
      <video>Video how it works</video>
    </div>
    <div class="flex justify-center py-4">
      <button
        class="flex items-center py-2 px-4 bg-purple-500 hover:bg-pink-500 text-white font-semibold rounded-lg shadow-md transition duration-300 ease-in-out mr-4"
      >
        <Icon icon="mdi:wallet-bifold-outline" class="m-1" :before="true" />
        Wallet
      </button>
      <button
        class="flex items-center py-2 px-4 bg-purple-500 hover:bg-pink-500 text-white font-semibold rounded-lg shadow-md transition duration-300 ease-in-out"
      >
        <Icon icon="mdi:telegram" class="mr-1" :before="true" />
        Contact me
      </button>
    </div>
  </main>
</template>
