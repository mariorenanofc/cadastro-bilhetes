<template>
    <div>
        <button @click="ativar">Sortear</button>
        <span v-show="ativou">Sorteado</span>
    </div>
</template>

<script>
    export default {
        name: 'Reutilizacao',
        data() {
            return {
                ativou: false
            }
        },
        methods: {
            ativar() {
                this.ativou = !this.ativou
            }
        }
    }
</script>

<style scoped>
    *{
        padding: 0;
        margin: 0;
        box-shadow: 0;
    }

    body {
        display: flexbox; 
        justify-content: center;
        align-items: center;
    }

    div {
        display: flexbox;
        margin: 0;
        max-width: 100%;
        height: 80px;
        background-color: red;
    }

    div button {
        width: 180px;
        height: 60px;
        align-items: center;
        justify-content: center;
        font-size: 28px;
        font-weight: 800;
        border: none;
        border-radius: 10px;
        background-color: aquamarine;
        margin: 10px;
    }
</style>