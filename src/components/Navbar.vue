<template>
  <div class="navbar d-flex justify-content-end">
    <div
      @click="$emit('open-menu')"
      class="nav-link font-weight-bold mt-3 btn btn-primary"
    >
      Menu
    </div>
  </div>
</template>

<script>
export default {
  name: "navbar",
};
</script>

<style lang="scss">
.navbar {
  width: 100%;
  z-index: 333;
  .nav-link {
    color: #fff;
    cursor: pointer;
    border: 0;
  }
}
</style>