<script setup>
import { onMounted } from "vue";

let props = defineProps({
  active: String,
});

onMounted(() => {
  switch (props.active) {
    case "home":
      document.querySelector("#home path").classList.add("active");
      break;
    case "search":
      document.querySelector("#search path").classList.add("active");
      break;
    case "create":
      document.querySelector("#create path").classList.add("active");
      break;
    case "explore":
      document.querySelector("#explore path").classList.add("active");
      break;
    case "profile":
      document.querySelector("#profile path").classList.add("active");
      document.querySelector("#profile circle").classList.add("active");
  }
});
</script>

<template>
  <nav class="nav">
    <RouterLink class="nav__link" to="/">
      <svg
        id="home"
        width="24"
        height="25"
        viewBox="0 0 24 25"
        fill="none"
        xmlns="http://www.w3.org/2000/svg"
      >
        <path
          d="M4.5 21.5V9.5L2 11.5L12 3.5L22 11.5L19.5 9.5V21.5H4.5Z M9.5 15V21.5H14.5V15H9.5Z M4.5 21.5H19.5"
          stroke="#190A00"
          stroke-width="2"
          stroke-linecap="round"
          stroke-linejoin="round"
        />
      </svg>
    </RouterLink>
    <RouterLink class="nav__link" to="/search">
      <svg
        id="search"
        width="24"
        height="25"
        viewBox="0 0 24 25"
        fill="none"
        xmlns="http://www.w3.org/2000/svg"
      >
        <path
          d="M10.5 19.5C15.1944 19.5 19 15.6944 19 11C19 6.30558 15.1944 2.5 10.5 2.5C5.80558 2.5 2 6.30558 2 11C2 15.6944 5.80558 19.5 10.5 19.5Z M13.3284 7.67157C12.6046 6.94772 11.6046 6.5 10.5 6.5C9.39543 6.5 8.39543 6.94772 7.67157 7.67157 M16.6109 17.1109L20.8536 21.3535"
          stroke="#190A00"
          stroke-width="2"
          stroke-linejoin="round"
        />
      </svg>
    </RouterLink>
    <RouterLink class="nav__link" to="/create">
      <svg
        id="create"
        width="24"
        height="25"
        viewBox="0 0 24 25"
        fill="none"
        xmlns="http://www.w3.org/2000/svg"
      >
        <path
          d="M12 16.5L12 8.5 M21 14L21 11 M3 14L3 11 M7 3.5H5C3.89543 3.5 3 4.39543 3 5.5V7.5 M17 3.5H19C20.1046 3.5 21 4.39543 21 5.5V7.5 M17 21.5H19C20.1046 21.5 21 20.6046 21 19.5V17.5 M7 21.5H5C3.89543 21.5 3 20.6046 3 19.5V17.5 M13.5 3.5H10.5 M16 12.5L8 12.5 M16 12.5L8 12.5 M13.5 21.5H10.5"
          stroke="#190A00"
          stroke-width="2"
          stroke-linecap="round"
          stroke-linejoin="round"
        />
      </svg>
    </RouterLink>
    <RouterLink class="nav__link" to="/explore">
      <svg
        id="explore"
        width="26"
        height="27"
        viewBox="0 0 26 27"
        fill="none"
        xmlns="http://www.w3.org/2000/svg"
      >
        <path
          d="M13 25.5C19.6274 25.5 25 20.1274 25 13.5C25 6.87258 19.6274 1.5 13 1.5C6.37258 1.5 1 6.87258 1 13.5C1 20.1274 6.37258 25.5 13 25.5Z M18.088 8.41199L15.544 16.044L7.91199 18.588L10.456 10.956L18.088 8.41199Z"
          stroke="black"
          stroke-width="2"
          stroke-linecap="round"
          stroke-linejoin="round"
        />
      </svg>
    </RouterLink>
    <RouterLink class="nav__link" to="/profile">
      <svg
        id="profile"
        width="24"
        height="25"
        viewBox="0 0 24 25"
        fill="none"
        xmlns="http://www.w3.org/2000/svg"
      >
        <circle
          cx="12"
          cy="6.5"
          r="4"
          stroke="#190A00"
          stroke-width="2"
          stroke-linecap="round"
          stroke-linejoin="round"
        />
        <path
          d="M21 22.5C21 17.5294 16.9706 13.5 12 13.5C7.02944 13.5 3 17.5294 3 22.5"
          stroke="#190A00"
          stroke-width="2"
          stroke-linecap="round"
          stroke-linejoin="round"
        />
      </svg>
    </RouterLink>
  </nav>
</template>

<style scoped>
.nav {
  position: fixed;
  left: 0;
  bottom: 0;
  width: 100%;
  height: 55px;
  max-height: 55px;
  box-shadow: 0 0 3px rgba(0, 0, 0, 0.2);
  background-color: #ffffff;
  display: flex;
  overflow-x: auto;
}

.nav__link {
  display: flex;
  flex-direction: column;
  align-items: center;
  justify-content: center;
  flex-grow: 1;
  min-width: 50px;
  overflow: hidden;
}

.active {
  stroke: #ff6700;
}

a,
a:visited,
a:hover,
a:focus,
a:active {
  color: unset;
}
</style>
