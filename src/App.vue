<script setup lang="ts">
import { RouterLink, RouterView } from 'vue-router'
import { Suspense } from 'vue';
</script>

<template>
  <header>
    <!-- <div class="wrapper"> -->
    <div class="logo">
      <h1>GilTube</h1>

    </div>
    <nav>
      <RouterLink to="/">Home</RouterLink>
      <RouterLink to="/about">About</RouterLink>
    </nav>
    <!-- </div> -->
    <OverlayBadge value="4" severity="danger" class="inline-flex">
      <Avatar label="sex" size="large" />
    </OverlayBadge>
  </header>
  <Suspense>
    <RouterView />
  </Suspense>

</template>

<style scoped>
@media (min-width: 1024px) {}
</style>
