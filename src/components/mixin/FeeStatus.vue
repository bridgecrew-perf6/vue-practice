<template>
  <div>
    <h2>합산된 요금 : {{ totalMoney }} 원</h2>
    <button @click="addMoney(50)">50</button>
    <button @click="addMoney(100)">100</button>
    <button @click="addMoney(150)">150</button>
    <button @click="addMoney(200)">200</button>
  </div>
</template>

<script>
import useMoney from "../../composables/useMoney.js";
// import moneyMixin from "../../mixins/moneyMixins.js";
export default {
  name: "feeStatus",
  setup() {
    const { addMoney, totalMoney } = useMoney();
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
