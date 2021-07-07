<template>
  <div class="min-h-screen bg-gray-100">
    <div class="max-w-5xl m-auto">
      <Header />
      <Home />
    </div>
  </div>
</template>

<script>
import Home from "./views/Home.vue";
import Header from "./components/Header.vue";

export default {
  name: "App",
  components: {
    Header,
    Home,
  },
};
</script>

<style>
@import url("https://fonts.googleapis.com/css2?family=Dancing+Script:wght@700&family=Lexend:wght@400;500;700&display=swap");

* {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
  font-family: "Lexend", -apple-system, BlinkMacSystemFont, "Segoe UI", Roboto,
    Oxygen, Ubuntu, Cantarell, "Open Sans", "Helvetica Neue", sans-serif;
}
</style>
