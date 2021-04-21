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
      { id: 1, title: "todo one", complete: false, times:1, },
      { id: 2, title: "todo two", complete: true, times:1, },
      { id: 3, title: "todo three", complete: false, times:1, },
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
