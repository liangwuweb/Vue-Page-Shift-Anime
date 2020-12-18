<template>
  <div class="wrap">
    <navigation :menuOpen="menuOpen" />
    <navbar @open-menu="menuOpen = !menuOpen" />
    <div>
      <div class="homepage d-flex justify-content-center align-items-center">
        <h1 class="text-light">HOME</h1>
      </div>
    </div>
  </div>
</template>

<script>
import Navbar from "./Navbar";
import Navigation from "./Navigation";

export default {
  name: "homepage",
  data: function () {
    return {
      menuOpen: true,
    };
  },
  components: {
    Navbar,
    Navigation,
  },
};
</script>

<style lang="scss" scoped>
.homepage {
  width: 100%;
  height: 100vh;
  position: absolute;
  top: 0;
  left: 0;
}
</style>