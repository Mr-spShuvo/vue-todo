<template>
  <span class="bg-green-400 h-2 w-2 m-2 rounded-full"></span>
  <div class="flex-grow font-medium px-2">{{ title }}</div>
  <Button text="&times;" />
</template>

<script>
import Button from "./Button.vue";
export default {
  name: "Todo",
  components: { Button },
  props: {
    title: String,
  },
};
</script>

<style lang="scss" scoped></style>
