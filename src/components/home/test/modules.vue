<template>
  <div class>
    <div class="heading d-flex">
      <h5 class="my-3">Modules</h5>
      <div class="ml-auto my-auto">
        <svg xmlns="http://www.w3.org/2000/svg" width="15" height="15" viewBox="0 0 15 15" fill="none">
          <g opacity="0.8">
            <path
              d="M8.125 7.5C8.125 7.15482 7.84518 6.875 7.5 6.875C7.15482 6.875 6.875 7.15482 6.875 7.5C6.875 7.84518 7.15482 8.125 7.5 8.125C7.84518 8.125 8.125 7.84518 8.125 7.5Z"
              fill="#03293D"
              stroke="#03293D"
              stroke-linecap="round"
              stroke-linejoin="round"
              class="ml-auto"
            />
            <path
              d="M3.75 7.5C3.75 7.15482 3.47018 6.875 3.125 6.875C2.77982 6.875 2.5 7.15482 2.5 7.5C2.5 7.84518 2.77982 8.125 3.125 8.125C3.47018 8.125 3.75 7.84518 3.75 7.5Z"
              fill="#03293D"
              stroke="#03293D"
              stroke-linecap="round"
              stroke-linejoin="round"
            />
            <path
              d="M12.5 7.5C12.5 7.15482 12.2202 6.875 11.875 6.875C11.5298 6.875 11.25 7.15482 11.25 7.5C11.25 7.84518 11.5298 8.125 11.875 8.125C12.2202 8.125 12.5 7.84518 12.5 7.5Z"
              fill="#03293D"
              stroke="#03293D"
              stroke-linecap="round"
              stroke-linejoin="round"
            />
          </g>
        </svg>
      </div>
    </div>

    <div class="modules">
      <!-- <Module /> -->
      <Module :items="backlogItems" />
    </div>
  </div>
</template>
<script>
import Module from "../../addModules";
export default {
  components: {
    Module,
  },
  data() {
    return {
      newBacklogItem: "",
      backlogItems: ["Apply gredient colours on the dashboard sidenav"],
    };
  },
  mounted() {
    if (localStorage.backlogs) {
      this.backlogItems = JSON.parse(localStorage.getItem("backlogs"));
    } else {
      localStorage.setItem("backlogs", JSON.stringify(this.backlogItems));
    }
  },
};
</script>
<style scoped>
.modules {
  max-height: 80vh;
  overflow-y: auto;
  padding: 0 0.5rem;
}
.modules::-webkit-scrollbar {
  width: 4px !important;
}
.modules::-webkit-scrollbar-track {
  box-shadow: inset 0 0 5px #d3d3d3;
  border-radius: 10px;
}
.modules::-webkit-scrollbar-thumb {
  background: #c0c0c0;
  border-radius: 10px;
}
</style>
