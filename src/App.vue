<template>
  <Header/>
  <PrimeiroComponente/>
  <h2 class="paragrafo-pai">O dado de app é: {{ mensagem }}</h2>
  <LifeCycle/>
  <Pessoa/>
</template>

<script>
import Header from './components/Header.vue';
import PrimeiroComponente from './components/PrimeiroComponente.vue'
import LifeCycle from './components/LifeCycle.vue'
import Pessoa from './components/Pessoa.vue';

export default {
  name: 'App',
  components: {
    Header,
    PrimeiroComponente,
    LifeCycle,
    Pessoa
  },
  data() {
    return {
      mensagem: 'Bem-vindo ao meu projeto Vue!'
    }

  }

}
 
</script>

<style>
  body{
    background-color: #333;
    color: #fff;
  }

  a{
    color: red;
  }

  .teste{
    background-color: #000;
  }

  .paragrafo-pai{
    color: blue;
  }
</style>