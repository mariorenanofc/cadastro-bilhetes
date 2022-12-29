<template>
    <div>
        <h1>🍀 Polo da Sorte</h1>
        <p>Seja bem vindo {{ nome }} {{ profissao }}</p>
    </div>
</template>

<script>
    export default {
        name: 'PrimeiroComponente',
        data(){
            return {
                nome:"Matheus Rodrigues",
                profissao: "vamos aos negócios!"
            }
        }
    }
</script>