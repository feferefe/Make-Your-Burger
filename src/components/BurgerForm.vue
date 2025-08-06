<template>
    
    <div>
        <p>Componente de Mensagem</p>
        <div>
            <form id="burger-form">
                <!-- Input nome do cliente -->
                <div class="input-container">
                    <label for="nome">Nome do Cliente:</label>
                    <input type="text" id="npme" name="name" v-model="nome" placeholder="Digite seu nome">
                </div>
                <!-- Select Escolha seu pão -->
                <div class="input-container">
                    <label for="pao">Escolha o pão:</label>
                    <select name="pao" id="pao" v-model="pao">
                        <option value="">Selecione o seu pão</option>
                        <option value="integral">Integral</option>
                    </select>
                <div/>
                <!-- Select Escolha seu tipo de carne -->
                <div class="input-container">
                    <label for="carne">Escolha a carne do seu burger:</label>
                    <select name="carne" id="carne" v-model="carne" >
                        <option value="">Selecione o tipo de carne</option>
                        <option value="maminha">Maminha</option>
                    </select>
                    <!-- Select Selecione os complementos -->
                    <div class="input-container">
                    <label for="carne">Selecione os complementos:</label>
                    <div class="checkbox-container">
                        <input type="checkbox" name="complementos" v-model="complementos" value="salame">
                        <span>Salame</span>
                    </div>
                </div>
                <!-- Btn Criar meu burger -->
                <div class="input-container">
                    <input type="submit" class="submit-btn" value="Criar meu burger">
                </div>
                </div>
                </div>
            </form>
        <div/>
    </div>  
</div>

</template>

<script>
export default {
    name: "BurgerForm"

}

</script>

<style scoped>

    #burger-form {
        max-width: 500px;
        margin: 0 auto;
    }

    #input-container{
        display: flex;
        flex-direction: column;
    }

    label{
        font-weight: bold;
        margin-bottom: 15px;
        color: #222;
        padding: 5px 10px;
        border-left: 4px solid #FCBA03;
    }

    input, select {
        padding: 5px 10px;
        width: 300px;
    }

    #complementos-container {
        flex-direction: row;
        flex-wrap: wrap;
    }
</style>