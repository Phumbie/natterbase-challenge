<template>
  <div class="body">
    <div class="select" :style="{background:bgColor}" @click="showSelect = !showSelect">
      <p class="text-white my-auto">
        {{test}}
        <span>
          <svg
            xmlns="http://www.w3.org/2000/svg"
            width="6"
            height="4"
            viewBox="0 0 6 4"
            fill="none"
          >
            <path d="M3 4L0 0.999823L1.00047 0L3 2.00035L4.99953 0L6 0.999823L3 4Z" fill="white" />
          </svg>
        </span>
      </p>
    </div>
    <div class="options" v-if="showSelect">
      <div class="option-card">
        <input type="text" placeholder="Search name" />
        <div class="option-menu mt-1">
          <p class="my-2" @click="testVal('Pass')">Pass</p>
        </div>
        <div class="option-menu">
          <p class="my-2" @click="testVal('Failed')">Failed</p>
        </div>
        <div class="option-menu">
          <p class="my-2" @click="testVal('Retest')">Retest</p>
        </div>
        <hr class="m-0" />
        <div class="option-menu">
          <p class="my-2" @click="testVal('Untest')">Untest</p>
        </div>
      </div>
    </div>
  </div>
</template>
<script>
export default {
  data() {
    return {
      showSelect: false,
      test: "Pass",
      bgColor: `#4dbd98`,
    };
  },
  methods: {
    testVal(val) {
      this.$emit("show");
      if (val === "Pass") {
        this.test = val;
        this.bgColor = `#4dbd98`;
      } else if (val === "Failed") {
        this.test = val;
        this.bgColor = `#eb0e43`;
      } else if (val === "Retest") {
        this.test = val;
        this.bgColor = `#f15832`;
      }
      this.showSelect = false;
    },
  },
};
</script>
<style scoped>
* {
  --sucsess: #4dbd98;
  --danger: #eb0e43;
  --warning: #f15832;
}
p {
  color: #03293d;
  width: 100%;
}
.option-menu {
  width: 100%;
  padding: 0.1rem;
  transition: all 0.5s linear;
}
.option-menu:hover {
  background-color: rgba(232, 231, 234, 0.3);
  cursor: pointer;
}
.select {
  /* background-color: var(--success); */
  border-radius: 5px;
  padding: 0.5rem 1.5rem;
  border: 2px solid rgba(26, 12, 47, 0.5);
  height: 100%;
  cursor: pointer;
  position: relative;
  width: 7rem;
  text-align: center;
  transition: all 0.5 linear;
  /* font-weight: bold; */
}
.body {
  position: relative;
  /* width: 20%; */
}
.options {
  position: absolute;
  /* top: 0; */
  z-index: 1;
  left: -7rem;
  width: 13rem;
  transition: opacity 0.5s ease-in;
}
.option-card {
  border-radius: 5px;
  background-color: white;
  padding: 0.5rem;
  box-shadow: 0px 5px 20px rgba(0, 0, 0, 0.08);
  border: 0.5px solid #f2f2f2;
}
input {
  border: none;
  background-color: rgba(134, 63, 235, 0.06);
  padding: 0.5rem;
  border-radius: 5px;
  width: 100%;
  outline: none;
}
</style>