<template>
  <v-app>
    <v-main style="background: linear-gradient(to right, pink, lightblue);">
      <NavBar />
      <v-container class="d-flex flex-column justify-center align-center">
        <div class="text-h3 text-sm-h2 font-weight-light mb-12" :style="{ userSelect: 'none' }">{{ title }}</div>
        <ShortenerInput />
      </v-container>
    </v-main>
    
    <v-footer style="background: linear-gradient(to right, pink, lightblue);" class="justify-center align-center text-no-wrap" app>
      
      <a class="text-decoration-none text-pink-accent-2 ml-1" href="https://www.qdqqd.com/" target="_blank">柯艺云</a>

    </v-footer>
  </v-app>
</template>

<script setup lang="ts">
import NavBar from './components/NavBar.vue';
import ShortenerInput from './components/ShortenerInput.vue';

const title = location.hostname;
</script>

<style>
html {
  overflow-y: auto !important;
}
</style>

<style lang="scss" scoped>
.v-container {
  min-height: 80vh;
}
</style>
