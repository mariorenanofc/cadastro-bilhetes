<template>
    <div>
        <h1>Sobre: </h1>
        <p>{{ nome }}</p>
        <Form />
        <p v-show="mostrar_nome"> {{ status }}</p>
        <br>
        <p  v-if="esta_trabalhando">🟢 - Sistema Online</p>
        <p  v-else> 🟠 - Sistema Offline</p>

    </div>
</template>

<script>
import Form from './Form.vue'
    export default {
  components: { Form },
        name: '',
        data() {
            return {   
                nome: 'Aqui vamos estruturar e organizar os dados de seus clientes e seus bilhetes. Não se preocupe vamos deixar tudo mais simples. 😉',
                esta_trabalhando: false,
                mostrar_nome: true,
                status: 'Você esta logado!'
                
            }
        }
    }
</script>