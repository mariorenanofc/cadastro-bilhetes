<template>
    <h1> {{ name }}</h1>
</template>

<script>
    export default {
        name: 'LifeCycle',
        data(){
            return {
                name: ''
            }
        },
        created() {
            setTimeout(() => {
                this.name = 'Mario Renan';
            }, 1000)
        },
        mounted() {
            setTimeout(() => {
                this.name = 'João Pedro';
            }, 300)
            
        }
    }
</script>