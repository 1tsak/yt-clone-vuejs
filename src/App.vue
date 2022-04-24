<template>
  <div class="main">
    <SideBar />
    <div class="body">
      <TopBar/>
      
    </div>
  </div>
</template>

<script>
import SideBar from "./components/SideBar.vue";
import TopBar from "./components/TopBar.vue";
// import MenuIcon from "vue-material-design-icons/Menu.vue";
// import Home from "vue-material-design-icons/Home.vue";

export default {
  name: "App",
  components: { SideBar, TopBar },
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

.body {
  width: 85vw;
  height: 100vh;
  background-color: #212121;
}

.nav-icons {
  color: white;
  margin-right: 10px;
}
.searchbar {
  justify-content: start;
  width: 40vw;
  height: 5vh;
  display: flex;
  border: 1px solid #484848;
  margin-top: 10px;
  margin-left: 15vw;
}
.search-input {
  height: 100%;
  background: #212121;
  margin-left: 25px;
  width: 35vw;
  border: none;
  color: gray;
}
.topbar {
  height: 8vh;
  display: flex;
  background: #212121;
  border-bottom: 1px solid rgba(68, 68, 68, 0.542);
}
.topbar-options {
  display: flex;
  margin-left:auto;
}
</style>
