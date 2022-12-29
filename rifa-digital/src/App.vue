
<script>
import Info from './components/Info.vue'
import PrimeiroComponente from './components/PrimeiroComponente.vue'
import LifeCycle from './components/LifeCycle.vue';
import Pessoa from './components/Pessoa.vue'
  export default{
  
  components: { 
    PrimeiroComponente,
    LifeCycle,
    Pessoa,
    Info
  },
  name: 'App',
  }
</script>

<template>
  <div>
    <PrimeiroComponente />
    <LifeCycle />
    <Pessoa />
    <Info  />
  </div>
</template>