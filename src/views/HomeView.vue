<script setup>
import Navigation from "../components/Navigation.vue";

let active = "home";
</script>

<template>
  <div class="main">
    <h1>Leisur</h1>
    <RouterLink to="/messages"
      ><img src="../assets/messages.png" alt="messages"
    /></RouterLink>
  </div>
  <div class="box">
    <div class="header">
      <div class="profile">
        <img src="../assets/niels.png" alt="Niels" />
        <div class="name">
          <h2>Niels Verdickt</h2>
          <p>@niels_verdickt</p>
        </div>
      </div>
      <button class="button--participate">Participate</button>
    </div>
    <h2 class="event--title">Tennis initiation</h2>
    <div class="event--info">
      <div class="event--location">
        <img src="../assets/location.svg" alt="location" />
        <h3>De Berken, Westrode</h3>
      </div>
      <div class="event--date">
        <img src="../assets/calendar.svg" alt="date" />
        <h3>06/06/2022</h3>
      </div>
      <p>
        Always wanted to play some tennis? I am Niels and I give tennis lessons
        for over 5 years. Monday the 6th of June I give an initation lesson.
        Feel free to join!
      </p>
      <img class="event--image" src="../assets/tennis.svg" alt="tennis" />
    </div>
  </div>
  <Navigation :active="active"/>
</template>

<style scoped>
h1 {
  font-family: "corner-store-jf", sans-serif;
  font-weight: 400;
  font-style: normal;
  font-size: 36px;
}

.box {
  margin-top: 2em;
  position: absolute;
  width: 390px;
  height: 522px;
  left: 0px;
  top: 135px;
  background: #ffffff;
  box-shadow: 0px 3px 10px 4px rgba(0, 0, 0, 0.16);
  border-radius: 5px;
}

.event--image {
  position: absolute;
  left: 0px;
  top: 303px;
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

.header {
  display: flex;
  flex-direction: row;
  align-items: center;
  justify-content: space-between;
  margin-top: 1.5em;
  margin-left: 1em;
  margin-right: 1em;
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
