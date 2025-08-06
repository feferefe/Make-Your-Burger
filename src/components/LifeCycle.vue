<template>
    <h1>Meu nome é: {{ nome }}</h1>
</template>

<script>
    export default {
        name:'LifeCycle',
        data() {
            return {
                nome:'Ainda não sei'
            }
        },
        created() {
            setTimeout (() => {
                // Simulando uma requisição para buscar o nome
                this.nome = 'Fernanda'
            }, 1000)
            
        },
        mounted() {

             setTimeout (() => {
                // Simulando uma requisição para buscar o nome
                this.nome = 'Fernanda Silva'
            }, 2000)
            this.lifeCycle();
        },
        methods:{
            lifeCycle(){
                console.log('Executou')
            }
        }

    }
</script>