<script setup>
import Navigation from "../components/Navigation.vue";
let active = "profile";
</script>

<template>
  <h1>My profile</h1>
  <img class="settings" src="../assets/settings.svg" alt="settings" />
  <img src="../assets/sennegroot.svg" alt="senne" />
  <h2>Senne Christiaens</h2>
  <p class="profile--bio">
    Hybrid Developer and Designer @ Thomas More Mechelen
  </p>
  <p class="profile--location">Antwerp, Belgium</p>
  <div class="tile">
    <div>
      <p>Created</p>
      <h3>21</h3>
    </div>
    <div>
      <p>Connections</p>
      <h3>940</h3>
    </div>
    <div>
      <p>Participated</p>
      <h3>87</h3>
    </div>
  </div>

  <div class="box">
    <div class="header">
      <div class="profile">
        <img src="../assets/senneklein.svg" alt="Senne" />
        <div class="name">
          <h2>Senne Christiaens</h2>
          <p>@senne_christiaens</p>
        </div>
      </div>
      <img src="../assets/pencil.svg" alt="pencil" />
    </div>
    <h2 class="event--title">Fitness workout</h2>
    <div class="event--info">
      <div class="event--location">
        <img src="../assets/location.svg" alt="location" />
        <h3>Basic-Fit, Kontich</h3>
      </div>
      <div class="event--date">
        <img src="../assets/calendar.svg" alt="date" />
        <h3>01/07/2022</h3>
      </div>
      <p>
        Looking for a gym partner to share my passion with. Age doesn’t matter.
        Motivation and being dedicated is the most important requisite!
      </p>
      <img class="event--image" src="../assets/fitness.svg" alt="fitness" />
    </div>
  </div>
  <Navigation :active="active" />
</template>

<style scoped>
h1 {
  font-family: "Merriweather", sans-serif;
  font-size: 20px;
  margin-bottom: 2em;
}

h2 {
  margin-top: 1em;
  margin-bottom: 1em;
  font-weight: 700;
  font-size: 16px;
}

.profile--bio {
  margin-left: 4em;
  margin-right: 4em;
  font-weight: 400;
  color: #ababab;
}

.profile--location {
  font-weight: 700;
  color: #ababab;
  margin-bottom: 1.5em;
}

.settings {
  position: absolute;
  left: 341.86px;
  top: 60.16px;
}

.tile {
  display: flex;
  flex-direction: row;
  justify-content: space-around;
  margin-bottom: 2.5em;
}

.tile p {
  color: #ababab;
}

.tile h3 {
  font-family: "Merriweather";
  font-weight: bolder;
  font-size: 20px;
  line-height: 0px;
}

.box {
  margin-left: -8px;
  margin-top: 0.5em;
  margin-bottom: 6em;
  padding-top: 0.1em;
  width: 390px;
  height: 518px;
  background: #ffffff;
  box-shadow: 0px 3px 10px 4px rgba(0, 0, 0, 0.16);
  border-radius: 5px;
}

.event--image {
  margin-bottom: -216.1px;
  margin-left: -18px;
  width: 390px;
}

.button--participate {
  background: #ffffff;
  border: 3px solid #ff6700;
  border-radius: 30px;
  font-family: "Lato";
  font-style: normal;
  font-weight: 700;
  font-size: 14px;
  color: #ff6700;
  padding: 5px 10px;
}

.active {
  background: #ff6700;
  border: 3px solid #ff6700;
  border-radius: 30px;
}

.header {
  margin-top: 1.5em;
}

.profile {
  display: flex;
  flex-direction: row;
}

.name {
  text-align: left;
  line-height: 0.3em;
  margin-left: 0.5em;
}

.name h2 {
  font-style: normal;
  font-weight: 700;
  font-size: 16px;
}

.name p {
  font-style: normal;
  font-weight: 700;
  font-size: 14px;
  color: #c4c4c4;
}

.event--title {
  text-align: left;
  margin-top: 1em;
  margin-left: 1em;
  font-size: 20px;
  color: #ff6700;
}

.event--info {
  margin-top: -25px;
  text-align: left;
  margin-left: 1.2em;
  font-size: 15px;
  color: #c4c4c4;
}

.event--info p {
  margin-left: 1em;
  margin-right: 1em;
  font-weight: 400;
  font-size: 16px;
  color: #ababab;
}

.event--location,
.event--date {
  margin-top: -25px;
  display: flex;
  color: #c4c4c4;
}

.event--location img {
  padding-left: 1px;
}

.event--location h3 {
  margin-left: 0.5em;
  font-weight: 400;
}

.event--date h3 {
  margin-left: 0.5em;
  font-size: 16px;
  color: #bdbdbd;
}
</style>
