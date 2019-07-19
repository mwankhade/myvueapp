<template>
  <div id="app">
    <div id="nav">
      <div class="navbar_menu">
          <router-link class="navbar_menu-item" to="/">Home</router-link>
          <router-link class="navbar_menu-item" to="/about">About</router-link>
          <router-link class="navbar_menu-item" to="/activityFeed">Activity Feed</router-link>
          <router-link class="navbar_menu-item" to="/leaderboard">Leaderboard</router-link>
          <router-link class="navbar_menu-item" to="/myProfile">My Profile</router-link>
        </div>
      </div>
    <router-view />
  </div>
</template>

<style>
#app {
  font-family: "Avenir", Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
}
#nav {
  background: #18181a;
  height: 100%;
  max-height: 100%;
  position: fixed;
  width: 15%;
}

#nav a {
  font-weight: bold;
  color: #b4b4be;
  text-decoration: none;
  display: block;
}

#nav a.router-link-exact-active {
  color: #fff;
}

.navbar_menu{
  line-height: 50px;
}

.navbar_menu-item {
  cursor: pointer;
  display: inline-block;
  font-family: Montserrat, sans-serif;
  font-size: 10px;
  font-weight: 700;
  margin: 0 0 0 25px;
  text-transform: uppercase;
}
</style>
