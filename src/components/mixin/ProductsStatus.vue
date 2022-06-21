<template>
  <div>
    <h2>전체 금액 : {{ totalMoney }} 원</h2>
    <div>
      <button @click="addMoney(100)">100</button>
      <button @click="addMoney(200)">200</button>
      <button @click="addMoney(300)">300</button>
      <button @click="addMoney(400)">400</button>
    </div>
  </div>
</template>

<script>
import useMoney from "../../composables/useMoney.js";
// import moneyMixin from "../../mixins/moneyMixins.js";
export default {
  name: "productStatus",
  setup() {
    const { addMoney, totalMoney } = useMoney();
    return {
      addMoney,
      totalMoney,
    };
  },
  // mixins: [moneyMixin],
  // data() {
  //   return {
  //     totalMoney: 3000,
  //   };
  // },
  // components: {},
};
</script>

<style></style>
