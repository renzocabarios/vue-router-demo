<script setup lang="ts">
import { RouterView } from "vue-router";
import router from "./routes";

const route = router;
const changeRoute = (url: string) => {
  route.push(url);
}
</script>
 
<template>
  <button @click="changeRoute('/')">1</button>
  <button @click="changeRoute('/2')">2</button>
  <button @click="changeRoute('/3')">3</button>
  <RouterView />
</template>

<style scoped>
</style>
