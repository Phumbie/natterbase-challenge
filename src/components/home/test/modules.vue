<template>
  <div class>
    <h5 class="my-3">Modules</h5>
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
