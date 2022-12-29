<template>
    <ul>
        <li><a href="#">Inicio</a></li>
        <li><a href="#">Cadastro</a></li>
        <li><a href="#">Sorteio</a></li>
    </ul>
</template>

<script>
    export default {
        name: 'Header'
    }
</script>

<style scoped>
    ul {
        list-style: none;
        display: flex;
        max-width: 100%;
    }

    li {
        margin-right: auto;
        font-size: 17px;
    }
    a {
        color: #ddd;
        text-decoration: none;
        transition: .5s;
    }

    a:hover {
        color: #f5fd1b;
        font-size: 18px;
        font-weight: 500;
    }
</style>