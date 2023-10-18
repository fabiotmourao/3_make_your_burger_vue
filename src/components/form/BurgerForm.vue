<template>
  <div>
    <p>Aqui vem as mensagens</p>
    <div>
      <form class="burger-form">
        <div class="input-container">
          <label for="nome">Nome do cliente</label>
          <input
            type="text"
            id="nome"
            name="nome"
            v-model="nome"
            placeholder="Digite o seu nome"
          />
        </div>

        <div class="input-container">
          <label for="pao">Escolha o tipo de pão:</label>
          <select name="pao" id="pao" v-model="pao">
            <option value="">Selecione o seu pão</option>
            <option value="integral">Integral</option>
          </select>
        </div>

        <div class="input-container">
          <label for="carne">Escolha a carne do seu burger</label>
          <select name="carne" id="carne" v-model="carne">
            <option value="">Selecione o tipo de carne</option>
            <option value="maminha">Maminha</option>
          </select>
        </div>

        <div id="opcionais-container" class="input-container">
          <label id="opcionais-title" for="opcionais">Escolha os opcionais:</label>
            <div class="checkbox-container">
                <input type="checkbox"  name="opcionais" v-model="opcionais" value="salame">
                <span>Salame</span>
            </div>
            
            <div class="checkbox-container">
                <input type="checkbox"  name="opcionais" v-model="opcionais" value="salame">
                <span>Salame</span>
            </div>
            
            <div class="checkbox-container">
                <input type="checkbox"  name="opcionais" v-model="opcionais" value="salame">
                <span>Salame</span>
            </div>
        </div>

        <div class="input-container">
          <input type="submit" class="submit-btn"  value="Criar meu Burger!">
        </div>
      </form>
    </div>
  </div>
</template>

<script>
export default {
  name: "BurgerForm",
};
</script>

<style scoped>
    .burger-form {
        max-width: 25rem;
        margin: 0 auto;
    }

    .input-container {
        display: flex;
        flex-direction: column;
        margin-bottom: 1.25rem;
    }

    label {
        font-weight: bold;
        margin-bottom: 0.7rem;
        color: #222;
        padding:  5px 10px;
        border-left:  4px solid #FCBA03;
    }

    input, 
    select {
        padding: 0.3re 10px;
        width: 300px;
    }

    #opcionais-container {
        flex-direction: row;
        flex-wrap: wrap;
    }

    #opcionais-title {
        width: 100%;   
    }

    .checkbox-container {
        display: flex;
        align-items: center;
        width: 50%;
        margin-bottom: 20px;
    }

    .checkbox-container span,
    .checkbox-container input {
        width: auto;
    }

    .checkbox-container span {
        margin-left: 6px;
        font-weight: bold;
    }

    .submit-btn {
        background-color: #222;
        color: #FCBA03;
        font-weight: bold;
        border:  2px solid #222;
        padding: 10px;
        font-size: 16px;
        margin: 0 auto;
        cursor: pointer;
        transition: .5s;
        border-radius: 6px;
    }

    .submit-btn:hover {
        background-color: #FCBA03;
        color: #222;
    }

</style>
