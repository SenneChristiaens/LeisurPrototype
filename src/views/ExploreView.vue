<script setup>
import Navigation from "../components/Navigation.vue";
let active = "explore";
</script>

<template>
  <h1 class="main">Explore</h1>
  <p class="intro">
    People you might want to connect with because they have similar interests!
  </p>

  <div class="flex">
    <div class="tile">
      <img src="../assets/sandra.svg" alt="Sandra" />
      <h2>Sandra More</h2>
      <p>I am 32 and always up for a game of tennis!</p>
      <button class="button--connect">+ Connect</button>
    </div>
    <div class="tile">
      <img src="../assets/pieter.svg" alt="Pieter" />
      <h2>Pieter Cox</h2>
      <p>Experienced web developer in node.js</p>
      <button class="button--connect">+ Connect</button>
    </div>
    <div class="tile">
      <img src="../assets/liena.svg" alt="Liena" />
      <h2>Liena Paeps</h2>
      <p>Studying IMD @ Thomas More Mechelen</p>
      <button class="button--connect">+ Connect</button>
    </div>
    <div class="tile">
      <img src="../assets/johan.svg" alt="Johan" />
      <h2>Johan Rossier</h2>
      <p>20 years old and a gym coach/addict</p>
      <button class="button--connect">+ Connect</button>
    </div>
    <div class="tile last">
      <img src="../assets/amelie.svg" alt="Amelie" />
      <h2>Amelie Heinrich</h2>
      <p>10y experienced Cook at The Jane.</p>
      <button class="button--connect">+ Connect</button>
    </div>
    <div class="tile last">
      <img src="../assets/emma.svg" alt="Emma" />
      <h2>Emma Rottger</h2>
      <p>Love to teach you some JavaScript</p>
      <button class="button--connect">+ Connect</button>
    </div>
  </div>

  <Navigation :active="active" />
</template>

<style scoped>
h1 {
  font-family: "Merriweather", sans-serif;
  font-size: 20px;
}

.flex {
  display: flex;
  flex-wrap: wrap;
  justify-content: space-around;
  margin-top: 20px;
}

.intro {
  text-align: left;
  margin-top: 1.5em;
  margin-left: 1.5em;
  margin-right: 2em;
  font-weight: 400;
  font-size: 16px;
  color: #ababab;
}

.tile {
  margin-bottom: 2em;
  padding-top: 1em;
  padding-bottom: 15.5em;
  width: 150px;
  height: 223px;
  background: #ffffff;
  box-shadow: 0px 3px 10px 4px rgba(0, 0, 0, 0.06);
  border-radius: 5px;
}

.tile img {
  width: 70px;
}

.tile h2 {
  font-weight: 700;
  font-size: 18px;
}

.tile p {
  padding-left: 1em;
  padding-right: 1em;
  font-weight: 400;
  font-size: 16px;
  color: #ababab;
}

.last {
  margin-bottom: 5em;
}
</style>
