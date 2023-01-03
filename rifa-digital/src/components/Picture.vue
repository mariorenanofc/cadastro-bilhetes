<template>
    <img :src="avatar" :alt="descricao" />
</template>

<script>
    export default {
        name: 'Picture',
        data() {
            return {
                avatar: "/img/logo.png",
                descricao: "Polo da Sorte"
            }
        }
    }
</script>

<style scoped>
    img {
        width: 180px;
    }
</style>