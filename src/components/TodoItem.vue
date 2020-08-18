<template>
    <div
    v-bind:class="{'is-complete':todo.compelted}"
    
    >
         
        <h3>{{todo.title}}</h3>
        </div>
</template>

<script>
export default {
    name:"TodoItem",
    props:['todo']
}
</script>

<style scoped>
.todo-item{
    background:#f4f4f4;
    padding:10px;
    border-bottom:1px #ccc dotted;
}

.is-complete{
    text-decoration: line-through;
}



</style>