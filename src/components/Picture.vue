<template>
    <div>
        <img :src="avatar" :alt="descricao">
        <MudarImagem @mudar-imagem="trocarImagem"/>
    </div>
</template>
<script>
import MudarImagem from './MudarImagem.vue';

export default {
    name: 'Picture',
    components: {
        MudarImagem
    },
    data() {
        return {
            avatar: '/img/maika.jpg',
            descricao: 'Foto da Maika Luiza'
        }
    },
    methods: {
        trocarImagem(){
            this.avatar = '/img/luizaamika.jpg'
        }
    }
}
</script>