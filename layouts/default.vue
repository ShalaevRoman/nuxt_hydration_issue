<script setup lang="ts">
const colorMode = useColorMode();
const toggleTheme = () => {
  colorMode.preference = colorMode.preference === 'dark' ? 'light' : 'dark';
};
</script>

<template>
  <div class="bg-amber-700 dark:bg-gray-800">
    <button @click="toggleTheme">Click</button>
    <NuxtImg
      :src="colorMode.preference === 'light' ? '1670484.jpg' : '1670488.jpg'"
      alt="pic"
      width="300"
      height="200"
    />
  </div>
</template>

<style scoped>

</style>