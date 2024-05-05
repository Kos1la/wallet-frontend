<script setup lang="ts">
import { RouterView } from 'vue-router'
import HeaderComponent from "@/components/HeaderComponent.vue";

</script>

<template>
  <div class="app">
  <HeaderComponent />
    <RouterView/>
  </div>
</template>



