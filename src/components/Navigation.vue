<template>
  <transition
    name="slide"
    enter-active-class="animate__animated animate__slideInLeft animate__faster"
    leave-active-class="animate__animated animate__slideOutLeft animate__faster"
  >
    <div v-if="menuOpen" class="navigation">
      <div
        class="container h-100 d-flex justify-content-center align-items-center"
      >
        <div class="text-center">
          <h3 class="font-weight-bold text-light">HOME</h3>
          <h3 class="font-weight-bold text-light">ABOUT</h3>
        </div>
      </div>
    </div>
  </transition>
</template>

<script>
export default {
  name: "navigation",
  props: ["menuOpen"],
};
</script>

<style lang="scss" scoped>
.navigation {
  width: 100%;
  height: 100%;
  background: #3ecc28;
  position: absolute;
  z-index: 111;
  top: 0;
  left: 0;

  h3 {
    cursor: pointer;
  }
}
</style>