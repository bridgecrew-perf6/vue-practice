<template>
  <div class="card">
    <div class="card-header"><slot name="header"></slot></div>
    <div class="card-body"><slot name="body"></slot></div>
    <div class="card-footer"><slot name="footer"></slot></div>
    <div><slot></slot></div>
  </div>
</template>

<script>
export default {};
</script>

<style scoped>
.card {
  box-shadow: 0 4px 8px 0 rgba(0, 0, 0, 0.3);
  transition: 0.3s;
  padding: 1rem;
  margin-bottom: 1rem;
  width: 200px;
}
.card-header {
  color: brown;
}
.card-body {
  color: bisque;
}
.card-footer {
  color: chocolate;
}
</style>
