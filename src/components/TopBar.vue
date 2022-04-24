<template>
  <div>
    <div class="topbar">
      <div class="searchbar">
        <input type="text" class="search-input" placeholder="Search" />
        <font-awesome-icon
          style="color: white; margin: 10px"
          :icon="['fas', 'magnifying-glass']"
        />
      </div>

      <font-awesome-icon
        style="
          color: white;
          margin: 20px;
          background-color: black;
          border-radius: 50%;
        "
        :icon="['fas', 'microphone']"
      />
      <div class="topbar-options">
        <font-awesome-icon
          style="
            color: white;
            margin: 20px;
            background-color: black;
            border-radius: 50%;
          "
          :icon="['fas', 'video']"
        />
        <font-awesome-icon
          style="
            color: white;
            margin: 20px;
            background-color: black;
            border-radius: 50%;
          "
          :icon="['fas', 'microphone']"
        />
        <font-awesome-icon
          style="
            color: white;
            margin: 20px;
            background-color: black;
            border-radius: 50%;
          "
          :icon="['fas', 'bell']"
        />
        <img
          style="height: 50px; padding: 10px; margin-top: 5px"
          src="../assets/logo.png"
        />
      </div>
    </div>
    <div class="topcat" >
      <div class="cat-items" v-for="cat in categories" :key="cat">
        <h1>{{cat}}</h1>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "TopBar",
  data() {
    return {
      categories: [
        "All",
        "Gadgets",
        "Computer Programming",
        "Computers",
        "NEET",
        "MCU",
        "Motivation",
        "Thrillers",
        "Gaming",
        "Google",
        "Photographs",
      ],
    };
  },
};
</script>

<style scoped>
.topcat {
  width: 85vw;
  height: 8vh;
  overflow-x: auto;
  white-space: nowrap;
  display: flex;
  align-items: center;
  border-bottom: 1px solid #484848;
}
.cat-items {
  background: rgba(255, 255, 255, 0.1);
  display: flex;
  padding: 0.3rem 0.7rem;
  margin: 5px;
  border-radius: 1rem;
  border: 0.5px solid rgba(255, 255, 255, 0.2);
  transition: background 150ms ease-out;
}
.cat-items:hover{
  background: rgba(255, 255, 255, 0.2);
}
.cat-items h1 {
  color: white;
  margin: auto;
  text-align: center;
  font-size: 16px;
  font-family: sans-serif;
}
</style>