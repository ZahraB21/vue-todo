<template>
  <div>
    <h1>Todos App</h1>
    <div v-for="todo in todos" v-bind:key="todo.id">
      <p>{{todo.title}}</p>
    </div>
  </div>
</template>

<script>
export default {
  name: "Todos",
  props: ["todos"],
};
</script>

<style scoped>
</style>