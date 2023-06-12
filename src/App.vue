<template>
  <div>
    <Home/><!-- create this after importing as a tag in this exact format-->
  </div>
</template>

<script setup>
import Home from "./components/Home/Home.vue"// the name Home must match the tag we have created up there inside a div in template
</script>

<style scoped>
.logo {
  height: 6em;
  padding: 1.5em;
  will-change: filter;
  transition: filter 300ms;
}
.logo:hover {
  filter: drop-shadow(0 0 2em #646cffaa);
}
.logo.vue:hover {
  filter: drop-shadow(0 0 2em #42b883aa);
}
</style>
