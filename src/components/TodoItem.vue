<template>
<div class="todo-item" v-bind:class="{'is-complete': todo.completed}">
    <h1> {{todo.title}}
        <input type="checkbox" v-on:change="markCheck"/>
    </h1>
    <button v-on:click="$emit('del-todo', todo.id)" class="del">x</button>
</div>
</template>
<script>

export default {
    name: "TodoItem",
    props: ['todo'],
    methods: {
        markCheck(){
            this.todo.completed = !this.todo.completed
        }
    }

}
</script>









<style scoped>
.todo-item {
    background: #f4f4f4;
    padding: 10px;
    border-bottom: 1px #ccc dotted;
}
.is-complete {
    text-decoration: line-through; 
}

 
</style>