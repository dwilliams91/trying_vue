<template>
    <div>
        <h1>To dos</h1>
        <div v-for="todo in todos" :key="todo.id">
            {{todo.title}}
        </div>
    </div>
</template>
<script>

export default ({
    name:'Todos',
    props:["todos"]
})
</script>
