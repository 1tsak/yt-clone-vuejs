<template>
  <div class="sidebar">
    <div class="sidebar-header">
      <font-awesome-icon
        style="margin-left: 25px; color: white; margin-right: 25px"
        :icon="['fas', 'bars']"
      />

      <img class="logo" src="../assets/yt_logo_rgb_dark.png" alt="" srcset="" />
    </div>
    <div class="nav-items-1">
      <button>
        <font-awesome-icon class="nav-icons" :icon="['fas', 'house']" />
        Home
      </button>
      <button>
        <font-awesome-icon class="nav-icons" :icon="['fas', 'compass']" />
        Explore
      </button>
      <button>
        <font-awesome-icon class="nav-icons" :icon="['fas', 'video']" />
        Shorts
      </button>
      <button>
        <font-awesome-icon class="nav-icons" :icon="['fas', 'rocket']" />
        Subscription
      </button>
    </div>
    <div class="nav-items-2">
      <button>
        <font-awesome-icon class="nav-icons" :icon="['fas', 'clapperboard']" />
        Library
      </button>
      <button>
        <font-awesome-icon
          class="nav-icons"
          :icon="['fas', 'clock-rotate-left']"
        />
        History
      </button>
      <button>
        <font-awesome-icon class="nav-icons" :icon="['fas', 'film']" />
        Your Videos
      </button>
      <button>
        <font-awesome-icon class="nav-icons" :icon="['fas', 'clock']" />
        Watch Later
      </button>
      <button>
        <font-awesome-icon class="nav-icons" :icon="['fas', 'angle-down']" />
        Show More
      </button>
    </div>
  </div>
</template>

<script>
export default {
    name:"SideBar"

};
</script>

<style scoped>
.logo {
  height: 1.25rem;
}
.nav-items-1 {
  display: flex;
  padding-top: 25px;
  padding-left: 0;
  flex-direction: column;
  border-bottom: 1px solid rgba(68, 68, 68, 0.542);
  padding-bottom: 15px;
}
.nav-items-2 {
  display: flex;
  padding-top: 25px;
  padding-left: 0;
  flex-direction: column;
  border-bottom: 1px solid rgba(68, 68, 68, 0.542);
  padding-bottom: 15px;
}
.nav-items-1 button {
  padding: 10px 10px 10px 15px;
  background: transparent;
  color: white;
  margin-left: 10px;
  border: none;
  text-align: start;
}
.nav-items-2 button {
  padding: 10px 10px 10px 15px;
  background: transparent;
  color: white;
  margin-left: 10px;
  border: none;
  text-align: start;
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
</style>