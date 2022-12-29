<template>
    <div>
        <h1>Sobre: </h1>
        <p>{{ nome }}</p>
        <Form />
    </div>
</template>

<script>
import Form from './Form.vue'
    export default {
  components: { Form },
        name: '',
        data() {
            return {   
                nome: 'Aqui vamos estruturar e organizar os dados de seus clientes e seus bilhetes. Não se preocupe vamos deixar tudo mais simples. 😉'
            }
        }
    }
</script>