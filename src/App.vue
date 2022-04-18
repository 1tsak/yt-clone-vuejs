<template>
  <div class="main">
    <div class="sidebar">
      <div class="sidebar-header">
        <MenuIcon
          style="margin-left: 25px; margin-right: 25px"
          fillColor="#FFFFFF"
        />

        <img
          class="logo"
          src="./assets/yt_logo_rgb_dark.png"
          alt=""
          srcset=""
        />
      </div>
      <div class="nav-items-1">
        <button>Home</button>
        <button>Explore</button>
        <button>Shorts</button>
        <button>Subscriptions</button>
      </div>
    </div>
    <div class="body"></div>
  </div>
</template>

<script>
import MenuIcon from "vue-material-design-icons/Menu.vue";

export default {
  name: "App",
  components: {
    MenuIcon,
  },
};
</script>

<style>
* {
  margin: 0;
  padding: 0;
}
.main {
  display: flex;
}
.sidebar {
  width: 15vw;
  height: 100vh;
  background-color: #212121;
}
.sidebar-header {
  display: flex;
  margin-top: 20px;
  justify-content: start;
  align-items: flex-start;
}
.body {
  width: 85vw;
  height: 100vh;
  background-color: #1e252c;
}
.logo {
  height: 1.25rem;
}
.nav-items-1{
  display: flex;
  flex-direction: column;
}
.nav-items-1 button {
  padding: 10px;
  background: transparent;
  color: white;
  border: none;
}
</style>
