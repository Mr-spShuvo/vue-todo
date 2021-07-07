<template>
  <header class="body-font">
    <div class="container mx-auto flex justify-between items-center p-5">
      <a
        class="
          flex
          items-center
          title-font
          font-medium
          items-center
          text-gray-900
          mb-4
          md:mb-0
        "
      >
        <img class="w-7" alt="Vue logo" src="../assets/logo.png" />
        <span class="ml-2 text-xl font-bold text-gray-600">Todo</span>
      </a>
      <Button text="&plus; Add Task" />
    </div>
  </header>
</template>

<script>
import Button from "../components/Button.vue";

export default {
  name: "Header",
  components: { Button },
};
</script>

<style lang="scss" scoped></style>
