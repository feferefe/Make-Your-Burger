<template>
    <Reutilizacao/>
    <h1>Olá vue!</h1>
    <Reutilizacao/>
    <p>{{ mensagem }}</p>
    <MultiplosEventos/>
    <Reutilizacao/>
    <Reutilizacao/>
    <Reutilizacao/>
    <Reutilizacao/>
    <Reutilizacao/>
    <Reutilizacao/>
</template>

<script>
import MultiplosEventos from './MultiplosEventos.vue';
import Reutilizacao from './Reutilizacao.vue';

    export default {
        name: 'PrimeiroComponente',
        components: {
            MultiplosEventos,
            Reutilizacao
        },
        data() {
            return{
                mensagem: 'Olá, este é o meu primeiro componente Vue!'
            }
        }
    }
</script>