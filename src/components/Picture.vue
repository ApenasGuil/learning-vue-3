<template>
    <img :src="avatar" :alt="descricao" />
    <!-- :src === v-bind:src (Modo enxuto)  -->
</template>

<script>
export default {
    name: "Picture",
    data() {
        return {
            avatar: "/img/avatar.png",
            descricao: "Guil Moraes",
        };
    },
};
</script>