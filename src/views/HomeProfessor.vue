<template>
    <NavReglus />
    <div class="container">
      <h1>Educador, Seja Bem Vindo!</h1>
      <div class="boxes">
        <div class="box blue">
          <div class="content">
            <h2>Agende reuniões com os estudantes</h2>
            <p class="small-text">Gratuito</p>
            <router-link to="/agenda" class="button">Agende</router-link>
          </div>
          <img src="@/assets/content/professorealuno.png" alt="Tutor" class="image" />
        </div>
  
        <div class="box purple">
          <div class="content">
            <h2>Acompanhe os seus estudantes</h2>
            <p class="small-text">Gratuito</p>
            <router-link to="/listaralunos" class="button">Acompanhe</router-link>
          </div>
          <img src="@/assets/content/organizeosestudos.png" alt="Organização" class="image" />
        </div>
      </div>
    </div>
  </template>
  
  <script>
  import NavReglus from "@/components/nav/NavReglusV2.vue";
  export default {
    name: "HomeProfessor",
    components: {
      NavReglus,
    }
}
  </script>
  
  <style>
  .container {
    text-align: center;
    margin: 2em;
  }
  
  .boxes {
    display: flex;
    justify-content: space-between;
    margin-top: 2em;
  }
  
  .box {
    width: 45%;
    padding: 1em;
    border-radius: 8px;
    color: white;
    display: flex;
    align-items: center;
    justify-content: space-between;
  }
  
  .blue {
    background-color: #8c52ff; /* Azul escuro */
  }
  
  .purple {
    background-color: #003366; /* Roxo */
  }
  
  .content {
    flex: 1;
    text-align: left;
  }
  
  .small-text {
    font-size: 0.8em;
  }
  
  .button {
    display: inline-block;
    padding: 0.5em 1em;
    margin-top: 0.5em;
    background-color: #ffffff;
    color: #000;
    border-radius: 4px;
    text-decoration: none;
    text-align: center;
  }
  
  .image {
    width: 100px; /* Ajuste o tamanho da imagem conforme necessário */
    height: auto;
  }
  </style>
  