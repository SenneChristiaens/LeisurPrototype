<template>
  <div class="main">
    <h1>Messages</h1>
    <img class="new--message" src="../assets/newmessage.svg" alt="newmessage" />
  </div>
  <div class="main search">
    <RouterLink to="/"
      ><img src="../assets/backorange.svg" alt="back"
    /></RouterLink>
    <input type="text" placeholder="Search" />
  </div>
  <div class="scroll">
    <div class="box">
      <div class="header">
        <div class="profile">
          <img src="../assets/liena.svg" alt="Liena" />
          <div class="name">
            <h2>Liena Paeps</h2>
            <p>Do you want to join me? · 2m</p>
          </div>
        </div>
      </div>
    </div>
    <div class="box">
      <div class="header">
        <div class="profile">
          <img src="../assets/bram.svg" alt="bram" />
          <div class="name">
            <h2>Bram Colleman</h2>
            <p>Yes, that would be breat! · 30m</p>
          </div>
        </div>
      </div>
    </div>
    <div class="box">
      <div class="header">
        <div class="profile">
          <img src="../assets/niels.svg" alt="niels" />
          <div class="name">
            <h2>Niels Verdickt</h2>
            <p>I would love to play some tennis! · 1h</p>
          </div>
        </div>
      </div>
    </div>
    <div class="box">
      <div class="header">
        <div class="profile">
          <img src="../assets/jay.svg" alt="Jay" />
          <div class="name">
            <h2>Jay Mills</h2>
            <p>Let's do a cooking course! · 3h</p>
          </div>
        </div>
      </div>
    </div>
    <div class="box">
      <div class="header">
        <div class="profile">
          <img src="../assets/peter.svg" alt="Peter" />
          <div class="name">
            <h2>Peter Willis</h2>
            <p>We have to reschedule 😞 · 3h</p>
          </div>
        </div>
      </div>
    </div>
    <div class="box">
      <div class="header">
        <div class="profile">
          <img src="../assets/sandra.svg" alt="Sandra" />
          <div class="name">
            <h2>Sandra More</h2>
            <p>See you tomorrow · 12h</p>
          </div>
        </div>
      </div>
    </div>
    <div class="box">
      <div class="header">
        <div class="profile">
          <img src="../assets/liena.svg" alt="Liena" />
          <div class="name">
            <h2>Pieter Cox</h2>
            <p>Had a lot of fun at your course · 15h</p>
          </div>
        </div>
      </div>
    </div>
    <div class="box">
      <div class="header">
        <div class="profile">
          <img src="../assets/liena.svg" alt="Liena" />
          <div class="name">
            <h2>Julie Miller</h2>
            <p>See ya!</p>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<style scoped>
h1 {
  font-family: "Merriweather", sans-serif;
  font-size: 20px;
}
.new--message {
  max-width: 26px;
}
.scroll {
  margin-top: 1em;
  overflow-y: scroll;
  height: 100%;
  max-height: calc(100vh - 15rem);
}

.search {
  margin-top: 1em;
}

.search input {
  background: #efefef;
  border: none;
  border-radius: 15px;
  width: 85%;
  height: 2.8em;
}

.search input::placeholder {
  padding-left: 1em;
  color: #bdbdbd;
}

.box {
  margin-left: auto;
  margin-right: auto;
  margin-top: 2em;
  width: 343px;
  height: 64px;
  background: #ffffff;
  box-shadow: 0px 3px 10px 4px rgba(0, 0, 0, 0.06);
  border-radius: 5px;
}

.profile {
  display: flex;
  flex-direction: row;
  margin-top: 7px;
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
</style>
