<template>
  <h1>Olá Vue! Isso é um componente dinânico</h1>
  <p>
    Meu nome é <code>{{ nome }}</code> e trabalho como
    <code>{{ profissao }}</code>
  </p>
</template>

<script>
export default {
  name: "PrimeiroComponente", // Definindo o nome do componente
  data() {
    // Todos os dados são declarados dentro de data()
    return {
      nome: "Guilherme",
      profissao: "Programador",
    };
  },
};
</script>
