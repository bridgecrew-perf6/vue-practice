<template>
  <div>
    <ul>
      <productItem
        v-for="product in products"
        :key="product.id"
        :product="product"
      />
    </ul>
  </div>
</template>

<script>
import productItem from "./ProductItem";
export default {
  name: "product-list",
  components: {
    productItem,
  },
  props: {
    products: {
      type: Array,
      default() {
        return [];
      },
    },
  },
};
</script>

<style></style>
