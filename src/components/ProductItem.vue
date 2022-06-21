<template>
  <li>
    <p calss="title">{{ product.name }}</p>
    <p calss="image">
      <img
        :src="`http://placeimg.com/200/100/any${product.id}`"
        :art="product.name"
      />
    </p>
    <p calss="price">{{ product.price }}</p>
  </li>
</template>

<script>
export default {
  name: "product-item",
  props: {
    product: Object,
  },
};
</script>

<style scoped>
li {
  border: 2px solid salmon;
  margin-bottom: 0.5rem;
}
.title {
  font-size: 24px;
  color: #2c82c9;
  font-weight: bold;
}
</style>
