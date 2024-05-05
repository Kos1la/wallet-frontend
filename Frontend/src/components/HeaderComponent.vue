<script setup lang="ts">
import { RouterLink } from 'vue-router'
</script>

<template>
  <header class="header">
    <div class="flex justify-center pt-4">
      <div class="max-w-5xl w-3/4">
        <nav class="md:text-lg text-md flex justify-between items-center">
          <div class="flex">
            <RouterLink class="" to="/">Home</RouterLink>
            <div class="border-l-2 border-b-pink-200 mx-2"></div>
            <RouterLink to="/wallet">Wallet</RouterLink>
          </div>
          <div>
            <RouterLink class="" to="/login">Login</RouterLink>
          </div>
        </nav>
        <hr class="border-t-2 border-b-pink-200 my-2 w-full" />
      </div>
    </div>
  </header>
</template>
