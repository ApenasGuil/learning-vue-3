<template>
    <p v-if="esta_trabalhando">Estou trabalhando no momento.</p>
    <p v-else>Estou em busca de novas oportunidades!</p>
    <p>Utilizo as seguintes tecnologias para back-end:</p>
    <ul>
        <li
            v-for="(technology, index) in backend_technologies"
            v-bind:key="index"
        >
            {{ technology }}
        </li>
<<<<<<< HEAD
    </ul>
    <p>Utilizo as seguintes tecnologias para front-end</p>
    <ul>
        <li v-for="technology in frontend_technologies" :key="technology.id">
            {{ technology.language }}
        </li>
=======
>>>>>>> bc627de9b895d733cd0a16c9e3d58739bb5d8165
    </ul>
    <div>
        <button @click="showEmail">{{ textoBotao }}</button>
    </div>
    <p v-show="mostrar_email">Mande uma mensagem para: {{ email }}</p>
    <p class="teste">
        Para acessar meu portifólio basta
        <a v-bind:href="meu_link" target="_blank">clicar aqui</a>
    </p>
    <Picture />
</template>

<script>
import Picture from "./Picture.vue";

export default {
    name: "Info",
    components: {
        Picture,
    },
    data() {
        return {
            esta_trabalhando: true,
            mostrar_email: false,
            email: "guilhermemoraes.dev@gmail.com",
            meu_link: "https://www.google.com",
            textoBotao: "Mostrar e-mail",
<<<<<<< HEAD
            backend_technologies: ["JavaScript", "Laravel", "Python"], // array
            frontend_technologies: [
                // array de objetos
                {
                    id: 1,
                    language: "HTML",
                },
                {
                    id: 2,
                    language: "CSS",
                },
                {
                    id: 3,
                    language: "Bootstrap",
                },
            ],
=======
            backend_technologies: ["JavaScript", "Laravel", "Python"],
>>>>>>> bc627de9b895d733cd0a16c9e3d58739bb5d8165
        };
    },
    methods: {
        showEmail() {
            this.mostrar_email = !this.mostrar_email;
            if (!this.mostrar_email) {
                this.textoBotao = "Mostrar e-mail";
            } else {
                this.textoBotao = "Esconder e-mail";
            }
        },
    },
};
</script>

<style>
.paragrafo-pai {
    color: red;
}
</style>