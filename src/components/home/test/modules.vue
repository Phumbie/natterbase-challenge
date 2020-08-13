<template>
  <div class>
    <h5 class="my-3">Modules</h5>
    <div class="modules">
      <Module v-for="i in 20" :key="i" class />
    </div>
  </div>
</template>
<script>
import Module from "../../addModules";
export default {
  components: {
    Module,
  },
};
</script>
<style scoped>
.modules {
  max-height: 85vh;
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