<template>
    <div>
        <header />
        <h1>🍀 Polo da Sorte</h1>
        <p>Seja bem vindo {{ nome }} {{ profissao }}</p>
        <MultiplosEventos />
        <life-cycle />
        <pessoa />
        <Form />
        <reutilizacao />
    </div>
</template>

<script>
import Form from './Form.vue';
import Header from './Header.vue';
import LifeCycle from './LifeCycle.vue';
import MultiplosEventos from './MultiplosEventos.vue';
import Pessoa from './Pessoa.vue';
import Reutilizacao from './Reutilizacao.vue';



export default {

    name: "PrimeiroComponente",
    components: { 
        MultiplosEventos, 
        Header, 
        LifeCycle, 
        Pessoa, 
        Form, 
        Reutilizacao },
    data() {
        return {
            nome: "Matheus Rodrigues",
            profissao: "vamos aos negócios!"
        };
    },
}
</script>