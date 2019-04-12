<template>
    <div class="todos">
        <div class="input">
            <ToDoInput msg="What would you like to do?" @add-todo="addToDo" />
        </div>
        <div class="todolist" v-for="todo in toDoList"> 
            <ul>
                <li>{{ todo.todo }}</li>
            </ul>
        </div>
    </div>
</template>

<script>
import ToDoInput from './ToDoInput.vue'

export default {
    name: 'ToDos',
    components: {
        ToDoInput
    },
    data() {
        return {
            toDoList: []
        }
    },
    methods: {
        addToDo(newToDo) {
            this.toDoList.push(newToDo);
            console.log(this.toDoList);
        }
    }
}
</script>

<style>
.todolist {
    text-align: center;
}
ul {
    list-style-type: none;
    padding: 0;
}
</style>