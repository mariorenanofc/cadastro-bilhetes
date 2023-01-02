<template>
    <div>
        <h1>🍀 Polo da Sorte</h1>
        <MultiplosEventos />
        <p>Seja bem vindo {{ nome }} {{ profissao }}</p>
    </div>
</template>

<script>
import MultiplosEventos from './MultiplosEventos.vue';



export default {

    name: "PrimeiroComponente",
    components: { MultiplosEventos },
    data() {
        return {
            nome: "Matheus Rodrigues",
            profissao: "vamos aos negócios!"
        };
    },
}
</script>