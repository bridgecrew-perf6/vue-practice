<template>
  <h2>Child Component</h2>
  <input type="text" v-model="username" />
</template>

<script>
export default {
  name: "childCmop",
  data() {
    return {
      username: "",
    };
  },
  methods: {
    sayHello() {
      console.log("say HELLO");
    },
  },
  beforeCreate() {
    console.log("child before create");
  },
  created() {
    console.log("child createed");
  },
  beforeMount() {
    console.log("child beforeMount");
  },
  mounted() {
    console.log("child Mounted");
  },
  beforeUpdate() {
    console.log("child beforeUpdate");
  },
  updated() {
    console.log("child updated");
  },
  beforeUnmount() {
    console.log("child beforeUnmount");
  },
  unmounted() {
    console.log("child unmounted");
  },
};
</script>

<style></style>
