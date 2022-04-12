<template>
    <h1>Meu nome é: {{ nome }} </h1>    
</template>
<script>

export default ({
    name: 'Lifecycle',
    data() {
        return {
        nome: 'Ainda não tem'
        }
    },
    created() {
        this.nome = 'Mateus'
    },
    mounted() {
        this.nome = 'Pedro'
    }

})
</script>
