<template>
  <div>
    <div class="home">
      <Sidebar />
      <Main />
    </div>
  </div>
</template>
<script>
import Navbar from "../layouts/navbar";
import Sidebar from "../layouts/sidebar";
import Main from "./main";
export default {
  components: {
    Navbar,
    Sidebar,
    Main,
  },
};
</script>
<style scoped>
.home {
  display: flex;
  height: 100vh;
  width: 100vw;
}
</style>
