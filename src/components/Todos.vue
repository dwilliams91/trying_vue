<template>
    <div>
        <h1>To dos components</h1>
        <h3>{{myText}}</h3>
    </div>
</template>
<script>
export default {
    name:'Todos',
    props:["myText"]
};
</script>
