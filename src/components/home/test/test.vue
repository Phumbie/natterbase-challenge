<template>
  <div class="test">
    <div class="test-box container-fluid">
      <!-- <div class="row"> -->
      <div class>
        <Module />
      </div>
      <div class>
        <TestCase />
      </div>
      <div class>
        <Quick />
      </div>
    </div>
    <!-- </div> -->
  </div>
</template>
<script>
import Module from "./modules";
import TestCase from "./Testcase";
import Quick from "./Quick";
export default {
  components: {
    Module,
    TestCase,
    Quick,
  },
};
</script>
<style scoped>
.test {
  width: 90%;
  margin: auto;
}
.test-box {
  display: grid;
  grid-template-columns: 20% 1fr 1fr;
  grid-gap: 1rem;
}
@media only screen and (max-width: 600px) {
  .test-box {
    display: block;
  }
}
</style>