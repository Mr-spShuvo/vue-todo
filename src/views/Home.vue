<template>
  <div class="w-full max-w-screen-xl mx-auto px-6">
    <div class="flex justify-center p-4 px-3 py-10">
      <div class="w-full max-w-md">
        <div class="bg-white shadow-md rounded-lg px-3 py-2 mb-4">
          <div
            class="
              block
              text-gray-600 text-center text-lg
              font-semibold
              py-4
              px-2
              border-b-2 border-solid
            "
          >
            📝 Todo List
          </div>
          <Todos :todos="todos" />
          <div
            class="
              bg-gray-200
              text-sm text-right
              py-3
              px-3
              -mx-3
              -mb-2
              rounded-b-lg
            "
          >
            <button
              class="hover:text-gray-600 text-gray-500 font-bold py-2 px-4"
            >
              Clear
            </button>
            <Button text="&plus; Add Task" />
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
import Button from "../components/Button.vue";
import Todos from "../components/Todos.vue";

export default {
  name: "Home",
  components: { Button, Todos },
  data() {
    return {
      todos: [],
    };
  },
  created() {
    this.todos = [
      {
        id: 1,
        title: "delectus aut autem",
        completed: false,
      },
      {
        id: 2,
        title: "quis ut nam facilis et officia qui",
        completed: false,
      },
      {
        id: 3,
        title: "fugiat veniam minus",
        completed: false,
      },
    ];
  },
};
</script>

<style lang="scss" scoped></style>
