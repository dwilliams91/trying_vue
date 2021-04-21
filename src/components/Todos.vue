<template>
  <div>
    <h1>To dos components</h1>
    <h3>{{ myText }}</h3>
    <ul id="example-1">
      <li v-for="item in myText" :key="item.id">
        {{ item.title }}
      </li>
    </ul>
  </div>
</template>
<script>
export default {
  name: "Todos",
  props: ["myText"],
  data(){
      return{
      options:[]
    }
  },
  mounted(){
      return fetch("http://localhost:8000/options",{
            headers: {
                "Authorization": `Token c22bbe51373f045d5d3efb26e53127fc51707541`
            }
        })
        .then(response=> response.json())
        .then(data=>this.options=data)
        .catch(err=> console.log(err.message))
  }
};
</script>
