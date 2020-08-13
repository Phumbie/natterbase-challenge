<template>
  <div class="main">
    <Navbar />

    <div class="body">
      <Homenav @display="display" />
      <Modules v-if="nav" />
      <div v-else>
        <Test />
      </div>
    </div>
  </div>
</template>
<script>
import Navbar from "../layouts/navbar";
import Modules from "./module";
import Test from "./test/test.vue";
import Homenav from "./Homenav";
export default {
  components: {
    Navbar,
    Modules,
    Test,
    Homenav,
  },
  data() {
    return {
      nav: true,
    };
  },
  methods: {
    display(val) {
      console.log(val);
      if (val === "modules") {
        this.nav = true;
      } else if (val === "tests") {
        this.nav = false;
      }
    },
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
