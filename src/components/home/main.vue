<template>
  <div class="main">
    <Navbar />
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
</style>
