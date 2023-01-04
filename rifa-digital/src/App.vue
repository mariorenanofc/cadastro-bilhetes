<template>
  <div>
    <Header />
    <PrimeiroComponente />
    <LifeCycle />
    <Pessoa />
    <Info :email="email" />
  </div>
</template>

<script>
import Info from './components/Info.vue'
import PrimeiroComponente from './components/PrimeiroComponente.vue'
import LifeCycle from './components/LifeCycle.vue';
import Pessoa from './components/Pessoa.vue'
import Header from './components/Header.vue';
  export default{
  
  components: { 
    PrimeiroComponente,
    LifeCycle,
    Pessoa,
    Info,
    Header
  },
  name: 'App',
  }
</script>


<style>
  body {
    background-color:#04b22a;
    color: rgb(250, 232, 232);
  }

  a {
    color: blue;
  }
</style>