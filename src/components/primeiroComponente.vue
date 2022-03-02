<template>
    <h1>Olá Vue! Isso é um componente dinânico</h1>
    <p>
        Meu nome é <code>{{ nome }}</code> e trabalho como
        <code>{{ profissao }}</code>
    </p>
    <MultiplosEventos />
    <Reutilizacao />
    <Reutilizacao />
    <Reutilizacao />
</template>

<script>
import MultiplosEventos from "./MultiplosEventos.vue";
import Reutilizacao from "./Reutilizacao.vue";
export default {
    name: "PrimeiroComponente", // Definindo o nome do componente
    components: {
        MultiplosEventos,
        Reutilizacao,
    },
    data() {
        // Todos os dados são declarados dentro de data()
        return {
            nome: "Guilherme",
            profissao: "Programador",
        };
    },
};
</script>
