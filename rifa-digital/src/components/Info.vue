<template>
    <div>
        <p>Para Acessar meu portifólio basta <a target="_blank" v-bind:href="meu_link">clicar aqui</a></p>
        <Picture />
    </div>
</template>

<script>
import Picture from './Picture.vue'
    export default  {
  components: { Picture },
        data() {
            return {
            meu_link: 'https://mariorenanofc.github.io/Portifo-lio/'
        }
        }
    }
</script>