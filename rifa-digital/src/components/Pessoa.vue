<template>
    <div>
        <h1>Sobre: </h1>
        <p>{{ nome }}</p>
        <Form />
        <p v-show="mostrar_nome"> {{ status }}</p>
        <br>
        <p  v-if="esta_trabalhando">🟢 - Sistema Online</p>
        <p  v-else> 🟠 - Sistema Offline</p>
        <button @click="showConteudo">{{ textoBotao }}</button>
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
                esta_trabalhando: true,
                mostrar_nome: false,
                status: 'Você esta logado!',
                textoBotao: 'Mostrar Situação'
                
            }
        },
        methods: {
            showConteudo(){
                this.mostrar_nome = !this.mostrar_nome
                if(!this.mostrar_nome) {
                    this.textoBotao = 'Mostrar Conteúdo'
                } else {
                    this.textoBotao = 'Esconder Situação'
                }
            }
        }
    }
</script>