<template>
    <div class="input">
        <div class="message">{{ msg }}</div>
        <div class="form">
            <form @submit.prevent="addToDo">
                <input type="text" v-model="todo">
            </form>
        </div>
    </div>
</template>

<script>
export default {
    name: 'ToDoInput',
    props: {
        msg: String
    },
    data() {
        return {
            todo: ''
        }
    },
    methods: {
        addToDo() {
            const newToDo = {
                todo: this.todo,
                completed: false
            }
            this.$emit('add-todo', newToDo);
            this.todo = '';
        }
    }
}
</script>

<style scoped>
.input {
    text-align: center;
    padding-top: 15px;
}
.message {
    font-size: 20px;
    padding-bottom: 15px;
}
input {
    border: none;
    border-bottom: 1px solid #d1d1e0;
    font-size: 20px;
    color: #2c3e50;
    text-align: center;
}
input:focus {
    outline: none;
}
</style>