<template>
    <div>
        <p>  {{ email}} </p>
        <p>Seguintes tecnólogias para Backend de Site:</p>
        <ul >
            <li v-for="(techlings, index) in backend_tecnologia" v-bind:key="index" >{{ techlings }}</li>
        </ul>
        <p>Seguintes tecnólogia para o FrontEnd do Site?</p>
        <ul>
            <li v-for="techlings in frontend_tecnologia" :key="techlings.id">{{ techlings.language }}</li>
        </ul>
        
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
            email: "mariorenan25@gmail.com",
            meu_link: 'https://mariorenanofc.github.io/Portifo-lio/',
            backend_tecnologia: ["Javascript","MySQL","Python"],
            frontend_tecnologia:[
                {id: 1, language: 'ScriptJS'},
                {id: 2, language: 'VueJS'},
                {id: 3, language: 'TypeScript'},
            ]
        }
        },
        props: {
            email: String
        }

    }

</script>