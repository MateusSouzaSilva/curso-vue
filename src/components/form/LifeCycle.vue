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
        setTimeout(() => {
        this.nome = 'Mateus'
    }, 1000);
    this.lifeCycle();
    },
    mounted() {
        this.nome = 'Pedro';
        this.lifeCycle();
    },
    methods: {
        lifeCycle() {
            console.log("Executou");
        }
    }

})
</script>
