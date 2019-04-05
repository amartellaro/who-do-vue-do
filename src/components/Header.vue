<template>
    <div class="header"><h1>{{ msg }}</h1></div>
</template>

<script>
export default {
    name: 'Header',
    props: {
        msg: String
    }
}
</script>

<style scoped>
.header {
    width: 100%;
    line-height: 50px;
    background-color: #f0f0f5;
    position: fixed;
    top: 0;
    margin: 0;
}
h1 {
    color: #5c5c8a;
    font-weight: 900;
    font-size: 70px;
    vertical-align: middle;
}
</style>