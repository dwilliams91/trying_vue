<template>
  <div>
    <h1>To dos components</h1>
    <h3>{{ myText }}</h3>
    <ul id="example-1">
      <li v-for="item in myText" :key="item.id">
        {{ item.title }} {{item.times}}
        <button v-on:click="item.times++">Click me</button>
      </li>
    </ul>
    
  </div>
  
</template>
<script>
export default {
  name: "Todos",
  props: ["myText"],

};
</script>
