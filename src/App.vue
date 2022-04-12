<template>
  <div>
    <Header />
    <PrimeiroComponente />
    <p>O dado de app é {{ testando }}</p>
    <lifecycle />
    <pessoa />
  </div>
</template> 
<script>
import PrimeiroComponente from './components/form/PrimeiroComponente.vue';
import Lifecycle from './components/form/LifeCycle.vue';
import Pessoa from './components/form/Pessoa.vue';
import Header from './components/form/Header.vue'

export default {
  name: 'App',
  components: {
    Header,
    PrimeiroComponente,
    Lifecycle,
    Pessoa
  },
  data() {
    return {
      testando: 'teste'

    }
  }  
}
</script>

<style>
  body {
    background-color: #333;
    color: #FFF;
  }
  a {
    color: blue;
  }
</style>