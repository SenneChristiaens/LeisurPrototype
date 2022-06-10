<script setup>
import Navigation from "../components/Navigation.vue";

let active = "search";
</script>

<template>
  <input type="text" placeholder="Search" />

  <p>Recent searches</p>
  <div class="flex">
    <div>
      <img src="../assets/sandra.svg" alt="sandra" />
      <div class="name">
        <h2>Sandra</h2>
        <h2>More</h2>
      </div>
    </div>
    <div>
      <img src="../assets/niels.svg" alt="Niels" />
      <div class="name">
        <h2>Niels</h2>
        <h2>Verdickt</h2>
      </div>
    </div>
    <div>
      <img src="../assets/bram.svg" alt="bram" />
      <div class="name">
        <h2>Bram</h2>
        <h2>Colleman</h2>
      </div>
    </div>
    <div>
      <img src="../assets/johan.svg" alt="johan" />
      <div class="name">
        <h2>Johan</h2>
        <h2>Rossier</h2>
      </div>
    </div>
  </div>

  <Navigation :active="active" />
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
  color: #bdbdbd;
}

input {
  text-indent: 2em;
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

h2 {
  font-style: normal;
  font-weight: 700;
  font-size: 16px;
}

.name {
  line-height: 0.3em;
}

.flex {
  margin-left: 2em;
  margin-right: 2em;
  display: flex;
  margin-top: 1em;
  justify-content: space-between;
}
</style>
