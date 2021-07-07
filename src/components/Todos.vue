<template>
  <div class="py-3 text-sm">
    <div
      class="
        flex
        justify-start
        items-center
        cursor-pointer
        text-gray-700
        hover:bg-gray-100
        rounded-md
        px-2
        py-2
        my-2
      "
      :key="todo.id"
      v-for="todo in todos"
    >
      <Todo :title="todo.title" />
    </div>
  </div>
</template>

<script>
import Todo from "./Todo.vue";
export default {
  name: "Todos",
  components: { Todo },
  props: {
    todos: Array,
  },
};
</script>

<style lang="scss" scoped></style>
