<template>
    <ul>
        <li><a href="#">Home</a></li>
        <li><a href="#">Projetos</a></li>
        <li><a href="#">Contato</a></li> 
        <li v-if="esta_logado">Meu Perfil</li>   
    </ul>
</template>
<script>
export default {
    name: 'Header',
    props: ["esta_logado"]
}
</script>
<style scoped>
    ul {
        list-style: none;
        display: flex;
        background-color: #999;
    }
    li {
        margin-right: 10px;
    }
    a {
        color: #000;
        text-decoration: none;
        transition: 0.5s;
    }
    a:hover {
        color: turquoise;
    }
</style>