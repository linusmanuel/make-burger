<template>
  <div>
    <p>Component de mensagem</p>
    <div>
      <form id="burger-form">
        <div class="input-container">
          <label for="nome">Nome do cliente</label>
          <input type="text" id="nome" name="nome" v-model="nome" placeholder="Digite seu nome">
        </div>
        <div class="input-container">
          <label for="nome">Escolha o pão</label>
          <select name="pao" id="pao" v-model="pao">
            <option value="">Selecione o seu pão</option>
            <option value="Integral">Integral</option>
          </select>
        </div>
        <div class="input-container">
          <label for="carne">Escolha a carne do seu Burger</label>
          <select name="carne" id="carne" v-model="carne">
            <option value="">Selecione o seu pão</option>
            <option value="Integral">Maminha</option>
          </select>
        </div>
        <div class="checkbox-container">
          <label id="opcionais-title" for="opcionais">Selecione os opcionais</label>
          <input type="checkbox" name="opcionais" v-model="opcionais">
          <span>Salame</span>
        </div>
        
        <div class="input-container">
          <input type="submit" class="submit-btn" value="Criar meu Burger">
        </div>
      </form>
    </div>

  </div>
</template>

<script>
  export default {
    name: 'BurgerForm',
  }
</script>

<style scoped>
  #burger-form {
    max-width: 400px;
    margin: 0 auto;
  }

  .input-container {
    display: flex;
    flex-direction: column;
    margin-bottom: 20px;
  }

  label {
    font-weight: bold;
    margin-bottom: 15px;
    color: #222;
    padding: 5px 10px;
    border-left: 4px solid #fcba03;    
  }

  input, select {
    padding: 5px 10px;
  }

  #opcionais-container {
    flex-direction: row;
    flex-wrap: wrap;
  }

  #opcionais-title {
    display: flex;
    align-items: flex-start;
    width: 50%;
  }

  .checkbox-container span,
  .checkbox-container input {
    margin-left: 6px;
    font-weight: bold;
  } 

  .submit-btn {
    background-color: #222;
    color: #fcba03;
    font-weight: bold;
    border: 2px solid #222;
    padding: 10px;
    margin: 0 auto;
    cursor: pointer;
    transition: .5s;
  }

  .submit-btn:hover {
    background-color: transparent;
    color: #222;
  }
</style>