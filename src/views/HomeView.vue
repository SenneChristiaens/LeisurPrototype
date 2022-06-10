<script setup>
import { onMounted } from "vue";
import Navigation from "../components/Navigation.vue";

let active = "home";
let button = document.querySelector(".button--participate");


let props = defineProps({
  active: String,
});

// button.addEventListener("click", () => {
//   console.log("clicked");
//   switch (props.active) {
//     case "participate":
//       button.classList.toggle("active");
//       button.innerHTML("Participating");
//       break;
//   }
// });
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
        <img src="../assets/niels.svg" alt="Niels" />
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
  <div class="box">
    <div class="header">
      <div class="profile">
        <img src="../assets/pieter.svg" alt="Pieter" />
        <div class="name">
          <h2>Pieter Cox</h2>
          <p>@pieter_cox</p>
        </div>
      </div>
      <button class="button--participate">Participate</button>
    </div>
    <h2 class="event--title">Node.JS Course</h2>
    <div class="event--info">
      <div class="event--location">
        <img src="../assets/location.svg" alt="location" />
        <h3>Online Zoom Course</h3>
      </div>
      <div class="event--date">
        <img src="../assets/calendar.svg" alt="date" />
        <h3>20/06/2022</h3>
      </div>
      <p>
        I work at Intracto and am a senior developer in Node.JS. This is my passion for over 20 years and I want to give other people the chance to see the power of Node.JS
      </p>
      <img class="event--image" src="../assets/node.svg" alt="node" />
    </div>
  </div>
    <div class="box last">
    <div class="header">
      <div class="profile">
        <img src="../assets/senneklein.svg" alt="Senne" />
        <div class="name">
          <h2>Senne Christiaens</h2>
          <p>@senne_christiaens</p>
        </div>
      </div>
      <img src="../assets/pencil.svg" alt="pencil">
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
        Looking for a gym partner to share my passion with. Age doesn’t matter. Motivation and being dedicated is the most important requisite!
      </p>
      <img id="last" class="event--image" src="../assets/fitness.svg" alt="fitness" />
    </div>
  </div>
  <Navigation :active="active" />
</template>

<style scoped>
h1 {
  font-family: "corner-store-jf", sans-serif;
  font-weight: 400;
  font-style: normal;
  font-size: 36px;
  margin: 0;
}

.box {
  margin-left: -8px;
  margin-top: 0.5em;
  margin-bottom: 3em;
  padding-top: 0.1em;
  width: 390px;
  height: 518px;
  background: #ffffff;
  box-shadow: 0px 3px 10px 4px rgba(0, 0, 0, 0.16);
  border-radius: 5px;
}

.last {
  margin-bottom: 6em;
}

#last {
  margin-bottom: -14.9em;
}

.event--image {
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
