<script setup>
import Navigation from "../components/Navigation.vue";
let active = "create";
</script>

<template>
  <h1>Create activity</h1>
  <img src="../assets/picture.svg" alt="picture" />
  <form action="">
    <label>Name</label>
    <input type="text" placeholder="Name" />
    <label>Location</label>
    <input type="text" placeholder="Online link or Adress" />
    <label>Date</label>
    <input type="text" placeholder="Date" />
    <img class="calendar" src="../assets/calendar_big.svg" alt="" />
    <label>Information</label>
    <textarea
      style="resize: none"
      cols="50"
      rows="7"
      placeholder="Add some extra information about the event..."
    ></textarea>
  </form>
  <RouterLink to="/"
    ><img class="button" src="../assets/button.svg" alt="button"
  /></RouterLink>
  <Navigation :active="active" />
</template>

<style scoped>
h1 {
  font-family: "Merriweather", sans-serif;
  font-size: 24px;
}

label {
  display: block;
  margin-left: 1em;
  text-align: left;
  font-weight: 700;
  font-size: 15px;
  line-height: 18px;
  color: #acacac;
}

input {
  margin-top: 0.5em;
  margin-bottom: 1em;
  text-indent: 1em;
  width: 339px;
  height: 55px;
  background: #ffffff;
  border: 3px solid #dfdfdf;
  border-radius: 15px;
}

textarea {
  padding-top: 1em;
  text-indent: 1em;
  margin-top: 0.5em;
  margin-bottom: 1em;
  background: #ffffff;
  border: 3px solid #dfdfdf;
  border-radius: 15px;
}

.button {
  margin-top: 2em;
}

.calendar {
  position: absolute;
  left: 83.08%;
  right: 11.79%;
  top: 48.84%;
  bottom: 44.79%;
}
</style>
