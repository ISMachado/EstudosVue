<template>
    <h1>Olá Vue!</h1>
    <p>Meu nome é {{ nome }} e trabalho com {{ profissao }}</p>
    <MultiplosEventos />
    <Reutilizacao />
</template>
  
<script> 
    import MultiplosEventos from './MultiplosEventos.vue'
    import Reutilizacao from './Reutilizacao.vue'

    export default {
        name: 'PrimeiroComponente',
        components: {
            MultiplosEventos,
            Reutilizacao
        },
        data() {
            return {
                nome: 'Igor',
                profissao: 'Programador'
            }
        }
    }   
</script>
