<template>
  <div>
    <PrimeiroComponente/>
    <p>O dado de app é {{ testando }}</p>
    <lifecycle />
    <pessoa />
  </div>
</template> 
<script>
import PrimeiroComponente from './components/PrimeiroComponente.vue';
import Lifecycle from './components/LifeCycle.vue';
import Pessoa from './components/Pessoa.vue';


export default {
  name: 'App',
  components: {
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