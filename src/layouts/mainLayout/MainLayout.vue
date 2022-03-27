<script setup lang="ts">
import AsideMenu from "@/layouts/mainLayout/AsideMenu.vue";

import { useRoute } from "vue-router";
const route = useRoute();
</script>

<template>
  <div class="main-layout">
    <AsideMenu />
    <main>
      <RouterView />
    </main>
  </div>
</template>

<style>
.main-layout {
  display: flex;
}
</style>
