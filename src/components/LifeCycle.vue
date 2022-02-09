<template>
    <h1>Meu nome é: {{ nome }}</h1>
</template>

<script>
export default {
    name: 'LifeCycle',
    data() {
        return {
        nome: 'Ainda não sei',
        }
    },
    created() {
        // Após a criação do componente, executa este método
        setTimeout(() => {
            this.nome = 'Guilherme'
        }, 1000);
    },
    mounted() {
        // Hierarquicamente abaixo do created, ou seja, é executado depois
        setTimeout(() => {
            this.nome = 'Pedro'
        }, 2000);
    }
};
</script>
