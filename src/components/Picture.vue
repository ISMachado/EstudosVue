<template>
    <img :src="avatar" :alt="descricao">
    <AlterarImagem @mudar-imagem="trocarImagem" />   
</template>

<script>
    import AlterarImagem from './AlterarImagem.vue'

    export default {
        name: "Picture",
        components: {
            AlterarImagem
        },
        data() {
            return {
                avatar: "/img/avatar.png",
                descricao: "Igor Machado"
            }
        },
        methods: {
            trocarImagem() {
                this.avatar = "/img/avatar2.png" 
            }
        }
    }
</script> 