<template>
    <header class="header"><h1>{{ msg }}</h1></header>
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
    background: #f0f0f5;
    text-align: center;
}
h1 {
    color: #5c5c8a;
    font-weight: 900;
    font-size: 70px;
    padding-top: 15px;
    padding-bottom: 15px;
    vertical-align: middle;
    margin: 0;
}
</style>