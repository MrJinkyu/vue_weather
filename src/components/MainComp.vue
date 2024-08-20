<template>
  <div class="container">
    <SearchBar />
    <Info />
  </div>
</template>

<script setup>
import Info from "./Info.vue";
import SearchBar from "./SearchBar.vue";
</script>

<style scoped lang="scss">
.container {
  padding: 20px;
}
</style>
