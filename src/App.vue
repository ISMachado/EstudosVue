<template>
  <div>
    <Header :esta_logado="true" />
    <PrimeiroComponente />
    <LifeCycle />
    <Info :email="Email" :esta_trabalhando=true />
  </div>
</template>
 
<script>
  import Header from './components/Header.vue'
  import PrimeiroComponente from './components/PrimeiroComponente.vue'
  import LifeCycle from './components/LifeCycle.vue'
  import Info from './components/Info.vue'

  export default {
    name: 'App',
    components: {
      Header,
      PrimeiroComponente,
      LifeCycle, 
      Info
    },
    data() {
      return {
        Email: 'igor@email.com'
      }
    }
  }
</script>

<!-- CSS Global -->
<style>
  body {
    background-color: #333;
    color:#FFF;
  }

  a {
    color: red;
  }
</style>