<template>
  <div id="app">
    <Todos v-bind:todos="todos" />
  </div>
</template>

<script>
import Todos from "./components/Todos.vue";

export default {
  name: "App",
  components: {
    Todos,
  },
  data() {
    return {
      todos: [
        { id: 1, title: "Todo 1", complete: false },
        { id: 2, title: "Todo 2", complete: true },
        { id: 3, title: "Todo 3", complete: false },
        { id: 4, title: "Todo 4", complete: true },
      ],
    };
  },
};
</script>

<style>
#app {
}
</style>
