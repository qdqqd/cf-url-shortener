<template>
  <div class="nav-bar">
    <v-btn
      v-tooltip:start="'看随机小姐姐扭扭扭'"
      density="compact"
      variant="text"
      icon="mdi-face-woman-shimmer"
      :size="32"
      @click="gotoGitHub"
    />
  </div>
</template>

<script setup lang="ts">
const gotoGitHub = () => {
  window.open('https://www.qdqqd.com/xjj/index.html', '_blank');
};
</script>

<style lang="scss" scoped>
.nav-bar {
  position: absolute;
  top: 8px;
  right: 8px;
}
</style>
