<script setup>
import { RouterView } from "vue-router";
import MainHeader from "./components/MainHeader.vue";
</script>

<template>
  <Suspense>
    <div>
      <MainHeader />
      <RouterView />
    </div>
  </Suspense>
</template>
