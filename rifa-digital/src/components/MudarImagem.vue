<template>
    <div>
        <button @click="$emit('mudarImagem')">Troca imagem da Logo</button>
    </div>
</template>

<script>
    export default {
        name: 'MudarImagem',
        emits: ['mudarImagem'],

        methods: {
            
        }
        
    }
</script>