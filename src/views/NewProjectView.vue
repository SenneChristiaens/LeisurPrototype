<script setup>
import Navigation from "../components/Navigation.vue";
let active = "create";
</script>

<template>
<h1>Create activity</h1>

<Navigation :active="active"/>
</template>

<style scoped>
h1 {
  font-family: "Merriweather", sans-serif;
  font-size: 24px;
}
</style>