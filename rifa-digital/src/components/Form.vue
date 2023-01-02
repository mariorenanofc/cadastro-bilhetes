<script >
import InputText from './form/InputText.vue';
import Submit from './form/Submit.vue';

    export default {
        name: 'Form',
        components: {
            InputText,
            Submit
        },
        data() {
            return {
                name: "",
                number: ""
            }
        },
        methods: {
            enviarformulario(e) {

                e.preventDefault();

                const name = this.name;
                const number = this.number;


                console.log("Seu nome é: " + name);
                console.log("Seu N/S é: " + number);
                console.log("Formulario Enviado");

                //Ajax

                // Inserir no banco de Dados
            }
        }
    }
</script>


<template>
    <div>
        <h2>Preencher dados</h2>
        <form action="" @submit="enviarformulario($event)">
       <div>
        <label for="name"></label>
        <input type="text" v-model="name" placeholder="Digite seu nome">
           <!--
            <InputText placeholder="Nome completo" />
            -->
       </div>
       <div>
        <input type="number" v-model="number" placeholder="Digite N/S" >
        <!--
            <label for="idBilhete"></label>
           <InputText type="number" placeholder="Número de Série" />
        -->
       </div>
       <div>
           <Submit />
       </div>
    </form>
    </div>
</template>
