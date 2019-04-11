<template>
    <div class="input">
        <div class="message">{{ msg }}</div>
        <div class="form">
            <form>
                <input type="text">
            </form>
        </div>
    </div>
</template>

<script>
export default {
    name: 'ToDoInput',
    props: {
        msg: String
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
}
input {
    border: none;
    border-bottom: 1px solid #d1d1e0;
}
input:focus {
    outline: none;
}
</style>