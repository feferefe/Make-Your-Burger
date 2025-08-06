<template>
    <h2>Meu Formulário:</h2>
    <form action="" @submit="enviarFormulario($event)">
        <div><input type="text" v-model="nome"></div>
        <div><input type="text" v-model="email"></div>
        <div><Submit/></div>
    </form>
</template>

<script>
import InputText from './form/InputText.vue'
import Submit from './form/submit.vue'

    export default {
        name: 'Form',
        components:{
            InputText,
            Submit
        },
        data() {
            return{
                nome: "",
                email: ""
            }
        },
        methods: {
            enviarFormulario(e) {

                e.preventDefault();

                const nome = this.nome;
                const email = this.email;

                console.log('Formulário enviado')
                console.log('O nome é ' + nome)
                console.log('O email é ' + email)
            }
        }
    }
</script>