<template>
    <div>
        <button @click="primeiro(txt1, $event), segundoEvento(txt2, $event), terceiroEvento()">Ativar Múltiplos eventos</button>
        <p>{{ multiplos_eventos }}</p>
    </div>
</template>
<script>
export default {
    name: 'MultiplosEventos',
    data() {
        return {
            multiplos_eventos: "",
            txt1: "Primeiro evento",
            txt2: "Segundo evento"
        }
    }, 
    methods: {
        primeiro(txt, e) {
            this.multiplos_eventos = txt;
        },
        segundoEvento(txt, e) {
            setTimeout(() => this.multiplos_eventos = txt, 500);
        },
        terceiroEvento() {
            setTimeout(() => this.multiplos_eventos= "", 1500);
        }
    }
}
</script>
<style scoped>
    div {
        margin:100px;
    }
</style>