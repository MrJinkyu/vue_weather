<script setup>
import Navbar from "./components/Navbar.vue";
import MainComp from "./components/MainComp.vue";
import { onMounted } from "vue";
import { useStore } from "vuex";
import About from "./components/About.vue";

const store = useStore();
onMounted(() => {
  store.dispatch("getWeather");
});
</script>

<template>
  <Navbar />
  <MainComp v-if="!$store.state.toggle" />
  <About v-else />
</template>

<style scoped lang="scss"></style>
