<template>
  <div id="app" class="h-screen text-font-color pt-12">
    <!-- <div class="text-4xl">Vue3 Demo</div> -->
    <app-header></app-header>
    <router-view></router-view>
  </div>
</template>

<script lang="ts">
import { defineComponent } from 'vue';
import AppHeader from '@/components/elements/header.vue';

export default defineComponent({
  name: 'App',
  components: { AppHeader },
});
</script>

<style lang="scss">
body {
  @apply bg-gray-900;
}

#app {
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
}
</style>
