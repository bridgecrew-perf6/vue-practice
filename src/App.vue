<template>
  <div>
    <h2>Hello composition API</h2>
    <TestComponent />
  </div>
</template>

<script>
import TestComponent from "./components/composition/TestComponent.vue";
export default {
  name: "App",
  components: { TestComponent },
  data() {
    return {};
  },
};
</script>

<style></style>
