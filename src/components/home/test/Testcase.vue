<template>
  <div>
    <h5 class="my-3">Added Test Case</h5>
    <div class="tests">
      <div class="test-card">
        <div
          class="test-cases d-flex justify-content-between my-2"
          :class="{ 'apply-border': show }"
          v-for="i in 30"
          :key="i"
        >
          <p class="my-auto">Apply gredient colours on the navigation</p>
          <Select class="my-auto" @show="showBorder" />
        </div>
      </div>
      <div class="test-actions text-center mt-3">
        <button class="new">New Test Case</button>
        <button class="real-test">Test</button>
      </div>
    </div>
  </div>
</template>
<script>
import Select from "../../UI/select";
export default {
  components: {
    Select,
  },
  data() {
    return {
      show: false,
    };
  },
  methods: {
    showBorder() {
      console.log("Hi");
      this.show = true;
    },
  },
};
</script>
<style scoped>
p {
  /* font-weight: bold; */
  color: #03293d;
  font-size: 0.9rem;
}
.tests {
  height: 80vh;
  background-color: white;
}
/* .test-card div:first-of-type {
  border-left: 1px solid red;
} */
.test-card::-webkit-scrollbar {
  width: 4px !important;
}
.test-card::-webkit-scrollbar-track {
  box-shadow: inset 0 0 5px #d3d3d3;
  border-radius: 10px;
}
.test-card::-webkit-scrollbar-thumb {
  background: #c0c0c0;
  border-radius: 10px;
}
.test-card {
  background-color: white;
  border-radius: 5px;
  height: 70vh;
  padding: 1rem;
  overflow-y: auto;
  overflow-x: hidden;
}
/* .apply-border {
  border-left: 2px solid #f15832;
} */
button {
  width: 40%;
  margin: auto;
  margin: 0 10px;
  padding: 0.5rem;
  border-radius: 5px;
  border: none;
}
.new {
  background-color: #23b3e8;
  color: white;
}
.real-test {
  border: 1px solid #03293d;
  background: none;
}
</style>
