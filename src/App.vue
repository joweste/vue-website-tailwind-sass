<template>
  <div id="app">
    <AppMain />
    <!-- <div id="nav">
      <router-link to="/">Home</router-link> |
      <router-link to="/about">About</router-link>
    </div> -->
    <!-- <router-view /> -->
  </div>
</template>

<script>
import AppMain from "@/views/AppMain";
export default {
  name: "App",
  components: {
    AppMain,
  },
};
</script>

<style lang="scss">
@import "./assets/css/app.css";
</style>
