<template>
  <div>
    <h2 v-bind="$attrs">HELLO {{ username }}</h2>
    <h3>오늘 {{ numberofVisit }}번째</h3>
    <h3>사이트 이름은 {{ siteInfo.name }} 입니다.</h3>
  </div>
</template>
<script>
export default {
  name: "GreetingUser",
  inheritAttrs: false,
  props: {
    username: String,
    numberofVisit: {
      type: Number,
      default: 0,
    },
    siteInfo: {
      type: Object,
      default: () => {
        return { name: "-", teacher: "-" };
      },
    },
  },
};
</script>
<style scoped></style>
