<template>
  <div id="app">
    <h3>hi</h3>
    <Todos v-bind:myText="todos"></Todos>
  </div>
</template>

<script>
import Todos from './components/Todos.vue';
export default {
  name: "App",
 

  data() {
    return {
    todos: [
      { id: 1, title: "todo one", complete: false },
      { id: 2, title: "todo two", complete: true },
      { id: 3, title: "todo three", complete: false },
    ]
    }
  },

  components: {
    Todos
  },
  
  
  
};
</script>

<style>
</style>
