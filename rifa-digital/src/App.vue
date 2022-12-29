
<script>
import PrimeiroComponente from './components/PrimeiroComponente.vue'
import LifeCycle from './components/LifeCycle.vue';
  export default{
  
  components: { 
    PrimeiroComponente,
    LifeCycle
  },
  name: 'App',
  }
</script>

<template>
  <div>
    <PrimeiroComponente />
    <LifeCycle />
  </div>
</template>