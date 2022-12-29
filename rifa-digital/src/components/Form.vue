<script >
import InputText from './form/InputText.vue';
import Submit from './form/Submit.vue';

    export default {
        name: 'Form',
        components: {
            InputText,
            Submit
        }
    }
</script>


<template>
    <div>
        <h2>Preencher dados</h2>
        <form action="">
       <div>
        <label for="name"></label>
           <InputText placeholder="Nome completo" />
       </div>
       <div>
            <label for="idBilhete"></label>
           <InputText type="number" placeholder="Número de Série" />
       </div>
       <div>
           <Submit />
       </div>
    </form>
    </div>
</template>
