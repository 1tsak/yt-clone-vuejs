<template>
  <div class="main">
    <SideBar/>
    <div class="body">
      <div class="topbar">
        <div class="searchbar">
          <!-- <font-awesome-icon style="color:white;" :icon="['fas','magnifying-glass']"/> -->
          <input type="text" class="search-input" placeholder="Search">

        </div>

      </div>
    </div>
  </div>
</template>

<script>
import SideBar from "./components/SideBar.vue";
// import MenuIcon from "vue-material-design-icons/Menu.vue";
// import Home from "vue-material-design-icons/Home.vue";

export default {
  name: "App",
  components: { SideBar },
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
.searchbar{
  justify-content: start;
  width: 40vw;
  margin: 10px;
  height: 5vh;
  margin: auto;
  display: flex;
  border: 1px solid #484848;
}
.search-input
{
  height: 100%;
  background: #212121;
  margin-left: 25px;
  width: 40vw;
  border: none;
  color: gray;

}
.topbar{
  height: 8vh;
  background: #212121;
  border-bottom: 1px solid rgba(68, 68, 68, 0.542);
}
</style>
