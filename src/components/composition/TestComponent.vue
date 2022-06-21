<template>
  <h2>Hello Resuability</h2>
  <hr />
  <FeeStatus />
  <hr />
  <ProductsStatus />
  <hr />
  <SavingStatus />
</template>

<script>
import FeeStatus from "../mixin/FeeStatus.vue";
import ProductsStatus from "../mixin/ProductsStatus.vue";
import SavingStatus from "../mixin/SavingStatus.vue";
import {} from "vue";
export default {
  name: "TestComponent",
  components: { FeeStatus, ProductsStatus, SavingStatus },
  methods: {},
};
</script>

<style></style>
