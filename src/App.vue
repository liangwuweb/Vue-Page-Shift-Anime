<template>
  <div id="app">
    <homepage />
  </div>
</template>

<script>
// import Navbar from "./components/Navbar";
import Homepage from "./components/Homepage";
// import Navigation from "./components/Navigation";

export default {
  name: "App",
  // data: function () {
  //   return {
  //     menuOpen: false,
  //   };
  // },
  components: {
    Homepage,
    // Navbar,
    // Navigation,
  },
};
</script>

<style>
body {
  background: #292929;
}

#app {
  font-family: "Avenir", Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
}
</style>
