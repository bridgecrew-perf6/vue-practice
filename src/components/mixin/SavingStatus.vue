<template>
  <div>
    <h2>총 적금 : {{ totalMoney }} 원</h2>
    <button @click="addMoney(1000)">1000</button>
    <button @click="addMoney(2000)">2000</button>
    <button @click="addMoney(1150)">1150</button>
    <button @click="addMoney(2200)">2200</button>
  </div>
</template>

<script>
import useMoney from "../../composables/useMoney.js";
// import moneyMixin from "../../mixins/moneyMixins.js";
export default {
  name: "savingStatus",
  setup() {
    const { addMoney, totalMoney } = useMoney(5000);
    return {
      addMoney,
      totalMoney,
    };
  },
  // mixins: [moneyMixin],
  // data() {
  //   return {};
  // },
  // methods: {},
};
</script>

<style></style>
