<template>
    <div>
        <img :src="avatar" :alt="descricao" />
        <MudarImagem @mudar-imagem="trocarImagem" />
    </div>
</template>

<script>
import MudarImagem from './MudarImagem.vue';

    export default {
        name: 'Picture',
        components: {
        MudarImagem 
        },
        data() {
            return {
                avatar: "/img/logo.png",
                descricao: "Polo da Sorte"
            }
        },
        methods: {
            trocarImagem(){
                this.avatar = "/img/logo-sem-fundo.png"
            }
        }
    }
</script>

<style scoped>
    img {
        width: 180px;
    }
</style>