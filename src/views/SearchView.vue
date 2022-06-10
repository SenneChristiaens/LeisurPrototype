<script setup>
import Navigation from "../components/Navigation.vue";

let active = "search";
</script>

<template>
  <input type="text" placeholder="Search" />

  <p>Recent searches</p>
  <Navigation :active = "active" />
</template>

<style scoped>
input {
  background: #efefef;
  border: none;
  border-radius: 15px;
  width: 85%;
  height: 2.8em;
}

input::placeholder {
  padding-left: 1em;
  color: #bdbdbd;
}

p {
  text-align: left;
  margin-left: 2em;
  margin-right: 1em;
  font-weight: 400;
  font-size: 16px;
  color: #ababab;
}
</style>
