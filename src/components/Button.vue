<template>
  <button
    class="
      inline-flex
      items-center
      bg-green-500
      text-white
      border-0
      py-1
      px-3
      focus:outline-none
      hover:bg-green-600
      rounded
      text-base
      font-medium
    "
    @click="onClick()"
  >
    {{ text }}
  </button>
</template>

<script>
export default {
  name: "Button",
  props: {
    text: {
      type: String,
      default: "&plus; Add Task",
    },
  },

  methods: {
    onClick() {
      console.log("Button Clicked");
    },
  },
};
</script>

<style lang="scss" scoped></style>
