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
* {
  margin: 0;
  padding: 0;
}
body {
  background: black;
  color: white;
}
a {
  text-decoration: none;
}

:root {
  --margin-nav-li: 20px;
  --color-button: #cd0061;
}
</style>
