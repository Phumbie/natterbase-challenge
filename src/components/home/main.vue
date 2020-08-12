<template>
  <div class="main">
    <Navbar />
    <div class="body">
      <!-- <h1>Helo</h1> -->
    </div>
  </div>
</template>
<script>
import Navbar from "../layouts/navbar";
export default {
  components: {
    Navbar,
  },
};
</script>
<style scoped>
.main {
  /* width: calc(100% - 7rem); */
  width: 100%;
}
.body {
  background: #2d2d2d;
  opacity: 0.04;
  height: calc(100% - 6rem);
}
</style>
