<template>
  <div class="main">
    <Navbar />
    <div class="body">
      <Homebody />
    </div>
  </div>
</template>
<script>
import Navbar from "../layouts/navbar";
import Homebody from "./body";
export default {
  components: {
    Navbar,
    Homebody,
  },
};
</script>
<style scoped>
.main {
  /* width: calc(100% - 7rem); */
  width: 100%;
}
.body {
  background: rgba(45, 45, 45, 0.04);
  /* opacity: 0.04; */
  height: calc(100vh - 6rem);
  overflow-y: auto;
}
</style>
